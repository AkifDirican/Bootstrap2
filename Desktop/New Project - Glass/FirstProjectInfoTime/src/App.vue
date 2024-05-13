<template class="temp">
  <div class= "page">
    <div class="left">
      <form class="sort">
        <h1> Sort</h1>
        <input type="checkbox" > Price Low to High</input>
        <br>
        <input type="checkbox" > Price High to Low</input>
      </form>
      <form class="brandSearch">
        <h1> Brands</h1>
        <input placeholder="Search Brand"></input>
        <br>
        <input type="checkbox" > Select All </input>
        <br>
        <input type="checkbox" > OHara-Group </input>
      </form>
    </div>
    <div class = "mid">
      <div class= "squares">
        <div div v-for="index in 20" :key="index" class="square"> 
          <p>10.99</p>
          <p>["Trees"]</p>
          <p>OHara-Group</p>
          <button>Add</button>
        </div>
      </div>
    </div>
    <div class ="right"> A
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.sort{
  background-color: rgb(220, 110, 220);;
}
.brandSearch{
  background-color: rgb(220, 220, 110);;
}
.squares{
  display:flex;
  flex-direction:row;
  flex-wrap:wrap;
  width:406px;
  height:auto;
  border:solid;
  border-width:3px;
  border-color:black;
}
.square{
  background-color:pink;
  width: 100px;
  height: 150px;
  border:solid;
  border-color:black;
}

.right{
  width:200px;
  height:200px;
  background-color: blue;
}

.page{
  display: flex;
  flex-direction: row;
  gap: 20px;
}
</style>