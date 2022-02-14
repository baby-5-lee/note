# vue路由懒加载

```js
{
      path: '/about',
      name: 'about',
      // route level code-splitting
      // this generates a separate chunk (About.[hash].js) for this route
      // which is lazy-loaded when the route is visited.
     component: () => import('@/views/AboutView.vue')
}
```

## 原理

在需要访问的时候才加载路由组件，提供更好的用户体验，一般来说Home路由不用懒加载，其他路由用懒加载