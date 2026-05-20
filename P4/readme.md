# DIU - Practica 4, entregables
>>> Tenemos que pasarlo a react y si queremos realizamos el despliegue con figma make (ya hecho porque funciona). Establecer en el readme lo que queremos que las otras personas
>>> evaluen para que se nos evalue de manera correcta
>>> En la p3 se entregan las capturas de lo que tenemos hecho de figma make como captura.
>>>
>>> Capturas con todas las refactorizaciones y ademas subir el poyecto con todo el codigo react aqui al github 
>>>
>>> Customizar el nav para que cambie a donde queramos o si no lo especificamos en el readme para no complicarse
>>> 



## Explicación de las distintas Páginas y sus Códigos React

### Página de Colas Interactivas
Esta vista facilita la toma de decisiones en tiempo real dentro del recinto. El componente App.jsx actúa como orquestador principal, manteniendo los componentes visuales limpios y desacoplados.

```jsx
import { Header } from './components/Header';
import { FiltersSidebar } from './components/FiltersSidebar';
import { MapView } from './components/MapView';
import { TruckDetails } from './components/TruckDetails';
import { useFoodTruckFilters } from './components/useFoodTruckFilters';

export default function App() {
  const filters = useFoodTruckFilters();

  return (
    <div className="bg-[#0b0e0f] flex flex-col items-start relative size-full">
      <Header />
      <div className="flex-[780_0_0] min-h-px relative w-full flex justify-center gap-4 px-4">
        <FiltersSidebar {...filters} onReset={filters.resetFilters} />
        <MapView
          trucks={filters.filteredTrucks}
          selectedTruck={filters.selectedTruck}
          onSelectTruck={filters.setSelectedTruck}
        />
        <TruckDetails truck={filters.selectedTruck} />
      </div>
    </div>
  );
}
```

Arquitectura:

Estado Centralizado: El Custom Hook useFoodTruckFilters extrae la lógica de negocio, gestionando los filtros y el elemento activo.

Componentes Presentacionales: App.jsx distribuye los datos mediante props a tres bloques clave:

FiltersSidebar: Permite al usuario acotar la búsqueda.

MapView: Renderiza los puestos filtrados en un mapa interactivo y captura la selección.

TruckDetails: Muestra la información estratégica del puesto seleccionado.

## Página de reservas
### Resumen de la página de reservas

Este código muestra la página principal de reservas en React.

### `App`

```jsx
import { ReservationPage } from "./components/reservation/ReservationPage";

export default function App() {
  return <ReservationPage />;
}
```

`App` importa y carga directamente el componente `ReservationPage`, por lo que la aplicación muestra la página de reservas.

### `ReservationPage`

```jsx
export function ReservationPage() {
  const r = useReservation();

  return (
    <PageShell cartCount={r.selected.length}>
      <HeroSection />
      <MapSection r={r} />
      <SelectionSection r={r} />
      <FiltersSection r={r} />
    </PageShell>
  );
}
```

`ReservationPage` construye la página de reservas. Usa `useReservation()` para gestionar la lógica, como los elementos seleccionados y los filtros.

La página se mete dentro de `PageShell`, que actúa como contenedor principal y recibe el número de elementos seleccionados mediante `cartCount`.

Dentro se muestran varias secciones:

- `HeroSection`: presentación de la página.
- `MapSection`: zona o mapa de reservas.
- `SelectionSection`: elementos seleccionados.
- `FiltersSection`: filtros disponibles.

En resumen, `ReservationPage` organiza la página y conecta la lógica de reservas con los componentes visuales.

Flujo de Usuario (UX):
El usuario explora el festival a través del mapa y utiliza los filtros para buscar opciones (ej. colas más rápidas). Al seleccionar un punto en el mapa, el panel de detalles revela información crítica, siendo el tiempo de espera estimado el dato clave para minimizar los tiempos muertos y optimizar su experiencia.

## 🍔 Vista: Carta de Hamburguesas

Esta vista presenta el catálogo de productos interactivo. El componente raíz utiliza un patrón de diseño basado en proveedores de contexto (Context API) para mantener el código escalable y el estado global accesible.

**Arquitectura:**
* **Gestión de Estado Global (`AppProviders`):** Componente envoltorio (*wrapper*) que inyecta las dependencias y el estado global a toda la aplicación (ej. datos del carrito de la compra, lista de productos, temas visuales). Evita el *prop drilling* (pasar propiedades manualmente por cada nivel de componentes).
* **Estructura Principal (`AppLayout`):** Componente que define el esqueleto visual de la página. Se encarga de organizar los bloques principales de la interfaz (cabecera, cuadrícula de productos, pie de página) consumiendo el contexto proporcionado por su elemento padre.

**Flujo de Usuario (UX):**
El usuario explora la carta completa del festival de forma fluida. Gracias a la arquitectura de proveedores, cualquier interacción compleja —como añadir una hamburguesa al pedido o filtrar por alérgenos— actualiza el estado global de forma centralizada, reflejándose inmediatamente en toda la interfaz sin recargas de página.

### Componente Principal (`App.jsx`)

```jsx
import { AppProviders } from "./components/AppProviders";
import { AppLayout } from "./components/AppLayout";

export default function App() {
  return (
    <AppProviders>
      <AppLayout />
    </AppProviders>
  );
}
```

## Landing Page

Este código corresponde a la página principal de **Remake Champions Burguer**, hecha con React.

### `App.tsx`

El componente `App` monta la estructura principal de la página.

Importa varios componentes y los muestra en orden:

```tsx
<Navigation />
<Hero />
<Features />
<Quote />
<CTA />
<Footer />
```

También aplica un fondo oscuro y centra el contenido en una anchura máxima.

### `Navigation`

Es la barra superior de navegación.

Muestra el logo/nombre de la web y varios enlaces:

- Carta
- Historia
- Colas
- Reservas
- Pedir ahora

Algunos botones abren páginas externas de Figma en una nueva pestaña y el botón de historia hace scroll hasta la sección correspondiente.

### `Hero`

Es la sección principal de presentación.

Muestra el mensaje inicial de la web, una descripción del restaurante y botones como:

- Pedir mi hamburguesa
- Ver carta

También enseña una hamburguesa destacada con precio y valoración.

### `Features`

Muestra las características principales del proyecto.

Explica qué hace diferente al restaurante:

- Accesibilidad desde cualquier dispositivo.
- Producto local y de barrio.
- Entrega en unos 30 minutos.

### `Quote`

Es una sección de frase destacada.

Incluye una cita sobre la ambición de ser los mejores y aparece firmada por los fundadores.

También tiene el identificador `historia`, por eso el menú puede hacer scroll hasta esta parte.

### `Footer`

Es el pie de página.

Muestra el copyright:

```text
© 2026 Remake Champions Burguer
```

### Resumen final

La página está dividida en componentes reutilizables.  
`App` organiza toda la estructura, mientras que cada componente se encarga de una parte concreta: navegación, presentación, características, frase destacada y pie de página.
