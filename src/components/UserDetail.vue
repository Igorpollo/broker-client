<template>
  <div>
    <h3>Nome: {{name}}</h3>
    <ul id="example-1">
      <li v-for="item in messages">
        {{ item.text }}
      </li>
    </ul>
  </div>
  
</template>

<script>
import {HTTP} from '../http-common'

export default {
  name: 'UserDetail',
  data () {
    return {
      name: 'Igor',
      messages: []
    }
  },
  created () {
    HTTP.get('messages')
    .then(response => {
      this.messages = response.data
    })
    .catch(e => {
    })
  }
}
</script>
