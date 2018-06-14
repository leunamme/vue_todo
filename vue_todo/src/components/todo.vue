}}<template>
  <div class="hello">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key='index'> {{ index }}. {{ data.skill }} </li>
      </ul>

      <p>this are the tasks</p>


      <!--<p v-if="skills.lenght < 3">good</p>
      <p v-else>not good</p>-->

      <!-- <div v-bind:class="{ alert: showAlert }"></div>-->
    </div>
  </div>
</template>

<script>
export default {
  name: 'todo',
  data() {
    return {
      skills: [
        { 'skill': 'Finish Perfecting your Laravel Skills'},
        { 'skill': 'Perfect Your Vue.js Skills'},
        { 'skill': 'Perfect Codeigniter'},
        { 'skill': 'Learn Python To Begin Machine-Learning'}
      ],
      showAlert: true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.holder {
  background-color: #fff;
}

ul {
  margin: 0;
  padding: 0;
  list-style-type: none;
}

ul li {
  padding: 20px;
  font-size: 1.3em;
  background-color: #e0edf4;
  border-left: 5px solid #3eb3f6;
  margin-bottom: 2px;
  color: #3eb3f6;
}

p {
  text-align: center;
  padding: 30px 0;
  color: gray;
}

.container {
  box-shadow: 0px 0px 40px lightgray;
}
</style>
