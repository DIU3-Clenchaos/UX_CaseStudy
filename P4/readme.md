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
