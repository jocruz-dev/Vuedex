 <template>
  <div class="component">
    <table class="stats-table">
      <tr>
        <th >HEIGHT</th>
        <th >WEIGHT</th>
        <th >TYPE</th>
      </tr>
      <tr>
        <td id="height">{{pokeHeight/10}}m</td>
        <td id="weight">{{pokeWeight/10}}kg</td>
        <td id="type">{{pokeType}}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: 'PokeStats',
  props: {
    pokeWeight: Number,
    pokeHeight: Number,
    pokeType: String
  }
}
</script>

<style scoped>
* {
  --table-widht: 20vw;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.stats-table {
  background: white;
  width: var(--table-widht);
  box-shadow: 0 1px 1px rgba(0,0,0,0.12), 
              0 2px 2px rgba(0,0,0,0.12), 
              0 4px 4px rgba(0,0,0,0.12), 
              0 8px 8px rgba(0,0,0,0.12),
              0 16px 16px rgba(0,0,0,0.12);
}
</style>
