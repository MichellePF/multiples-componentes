.<template>
  <div class="wrap">
    <div id="miApp">
        <h3>{{titulo}}</h3>
        <div>
            <ul>
               <li v-for="(enlace, i) in enlaces" v-bind:key="i"><a v-bind:href="enlace.url">{{enlace.texto}}</a></li>
            </ul>
        </div>
    </div>
    
   
  </div>
</template>

<script>
export default {
    name: 'MiLista',
    props: {
        titulo: String,
        enlaces: Array
    }
   

}
</script>

<style scoped>
    .wrap {
    margin: auto;
    height: auto;
    width: 800px;
    text-align: center;
    border: 5px solid crimson;
    font-size: 25px;
    background-color: coral;
    color: white;
    }
    ul {
        list-style: none;
    }


</style>