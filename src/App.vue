<template>

  <Users/>
</template>

<script>
import Users from './components/Users.vue'
import UserForm from './components/UsersForm.vue'
const NotFound = { template: '<p>Page not found</p>' }
const routes = {
  '/': Users,
  '/form': UserForm
}
export default {
  name: 'App',
  components: {
    Users
  },
  data() {
    return {
      currentRoute: window.location.pathname
    }
  },

  computed: {
    ViewComponent () {
      return routes[this.currentRoute] || NotFound
    }
  },
  render (h) { return h(this.ViewComponent) }

}
</script>
