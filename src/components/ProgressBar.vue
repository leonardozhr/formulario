<template>

<div class="row">
        <div class="col-12 ">
            <h1 v-bind:about="porcentaje">Progreso del {{porcentaje}}%</h1>
    <div class="progress">
  <div class="progress-bar" role="progressbar" 
    :style="`width: ${porcentaje}%`" 
  :aria-valuenow="porcentaje"
   aria-valuemin="0" 
   aria-valuemax="100">{{porcentaje}}%</div>
</div>
</div>
</div>


</template>

<script>
    export default{
        props:{
            porcentaje:Number,

        }
    }
</script>