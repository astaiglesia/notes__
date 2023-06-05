# [Concurrent Rendering](https://www.udemy.com/course/concurrent-rendering-adventures-in-react-18/)


## react refreshers

fyi: *react 18 needs react-router v6*

<hr>

some of the features react 17 already added:

### `<Suspense />`
> **allows react to 'suspend' rendering of a component subtree**
> **fallback component** is rendered when a child/grandchild component is not ready to be rendered
> e.g. 
>   - ES bundle containing the componentisn't loaded yet
>   - data required for component rendering isn't available yet

suspense allows:
- fallback ocmponent replaces the complete child component tree
- suspends rendering when a promise is thrown
  - resumes when the promise resolves
- lazy loading of data
- nest and/or parallelize `<Suspense/>` components as needed


## `Using Suspense`

*SWR allows for easy use of suspense*

> - update ReactDOM.render() call in index.tsx
>   - wrap App with SWR Config with value prop assigned the SWR config
>   - add config property to `<SWRConfig />` => `suspense: true` 
>   - wrap with Suspense with fallback prop assigned the fallback/ loading component
>   - wrap with ErrorBoundary with FallbackComponent assigned the error fallback


<br>

### `<ErrorBoundary />`
- error handling while suspended


<br>

### `concurrent mode`

- what

- how


<br>

### `createRoot()`
- rendering a React 18 application


<br>

### `Orchestrating <Suspense /> boundaries using <SuspenseList />`



<br>

### `Using startTransition() and/or useTransition to defer work`




<br>
<br>
<hr>

## more stuff

