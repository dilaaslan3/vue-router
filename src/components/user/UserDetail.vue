<template>
  <div>
    <h3>Some User Details</h3>
    <p>User Loaded : {{$route.params.id}}</p>
    <!--:to="'/user/' + $route.params.id + '/edit'"-->
    <router-link
      tag="button"
      :to="{name:'userEdit', params:{id:$route.params.id}}"
      class="btn btn-primary"
    >Edit User</router-link>
  </div>
</template>
