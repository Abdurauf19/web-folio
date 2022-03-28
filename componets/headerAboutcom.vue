<template>
  <div>
    <div class="expirencee">
        <div class="expirence-number">
              <h3 class="expirence-number-num">{{Num}}</h3>
              <p class="expirence-number-text">{{Text}}</p>
        </div>
        </div>
  </div>
</template>


<script>
export default {
  props : {
     Num: {
      type:String,
    },
    Text: {
      type:String,
    },
  }
}
</script>


<style >
.expirencee {
  display: flex;

}
  .expirence-number-num {
  color: var(--blue-color);
  font-family: var(--font_E);
  font-size: 3.75rem;
  line-height: 4.125rem;
  margin: 0;
}

.expirence-number-text{
  font-family: var(--font_E);
  color:var(--textt-color);
  font-size: 1.31rem;
  line-height: 1.9375rem;
  margin: 0;
}
</style>