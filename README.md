# vue-3-demo

## Project setup
```
yarn install
yarn upgrade
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).




# app wide data without vuex

* display emails in table
* mark as read
* display dates
* sort and filter
* archive button

* to handle async (async setup)
* fallback renders if waiting on any async method
  <Suspense>
    <template #default>
      <MailTable />
    </template>
    <template #fallback>
      Loading...
    </template>
  </Suspense>

* jsonServer
* npm i -g json-server
json-server --watch db.json

# reactive
let emails = reactive(new Set())
