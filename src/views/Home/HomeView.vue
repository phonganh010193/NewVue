<template>
    <div class="container home-container d-flex flex-row m-0 p-0">
      <SideBar />
      <div class="home-content">
        {{ count }}
        <button @click="increment">Tăng</button>
        <button @click="december">giảm</button>
        <input v-model="name"/>
        <button @click="AddList">ThÊM</button> 
        <div class="list">
          <div class="list-item" v-for="(item, index) in list">
            <p>{{ item.title }}</p>
          </div>
        </div>
      </div>
    </div>
</template>
<script>
import { HTTP } from '@/http-common';
import SideBar from '../../components/sidebar/SideBar.vue';
import { get, ref } from 'firebase/database';
import { database } from '../../firebase';


  export default {
    components: {
        SideBar,
    },
    data() {
      return {
        data: [],
        count: 0,
        name: "",
        list:[
          {title: "pham van phong"}
        ]
      }
    },
    async created() {
      // HTTP.get(`posts`)
      //   .then(response => {
      //     this.posts = response.data;
      //     console.log('res', response.data)
      //   })
      //   .catch(e => {
      //     this.errors.push(e)
      //   })
      // }
      await get(ref(database, "Cart")).then((snapshot) => {
      if (snapshot.exists()) {
        this.data === snapshot.val();
        console.log(snapshot.val());
      }
      }).catch((error) => {
        console.error(error);
      });
    },
    methods: {
      increment() {
        this.count++
      },
      december() {
        this.count--
      },
      AddList() {
        console.log(this.name)
        this.list.push({title: this.name})
        this.name = "";
      }
    }
  }
</script>
<style >
    .home-container {
      width: 100%;
    }
    .home-content {
      width: 75%;
      margin-left: 30px;
    }
</style>