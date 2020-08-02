<template>
  <div class="box shadow rainbow" style="margin:0px auto;"> 
    <h1>Test</h1>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .box {
	width: 80%;
	height: 100px;
	background: rgb(94, 182, 194);
	border-radius: 10px;
	margin: 10px;
}

.shadow {
	position: relative;
	max-width: 90%;
	box-shadow: 0px 1px 4px rgba(0,0,0,0.3),
				0px 0px 20px rgba(0,0,0,0.1) inset;
}

.shadow::before,
.shadow::after {
   content:"";
   position:absolute;
   z-index:-1;
}

.shadow::before,
.shadow::after {
   content:"";
   position:absolute;
   z-index:-1;
   bottom:15px;
   left:10px;
   width:50%;
   height:20%;
}

.shadow::before,
.shadow::after {
   content:"";
   position:absolute;
   z-index:-1;
   bottom:15px;
   left:10px;
   width:50%;
   height:20%;
   box-shadow:0 15px 10px rgba(0, 0, 0, 0.7);
   transform:rotate(-1deg);
}

.shadow::after{
   right:10px;
   left:auto;
   transform:rotate(1deg);
 }

</style>
