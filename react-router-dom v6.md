#### App.tsx
```ts
import React from 'react';
import { RouterProvider } from 'react-router-dom';

import router from './Router';

const App = () => <RouterProvider router={router} />;

export default App;
```

#### Router.tsx
```ts
import React from 'react';
import { createBrowserRouter } from 'react-router-dom';

import { PokedexDetailPage, PokedexListPage } from './pages';

const router = createBrowserRouter(
  [
    {
      path: '/',
      children: [
        { index: true, element: <PokedexListPage /> },
        {
          path: ':id',
          element: <PokedexDetailPage />,
        },
      ],
    },
  ],
  { basename: '/2023-01-React-Study-Pokedex' },
);

export default router;
```
- createBrowserRouter 함수의 두번째 인자에서 basename을 설정할 수 있음