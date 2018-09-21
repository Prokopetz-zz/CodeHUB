<template>
    <form>
        <input id="input"
               :placeholder="text"
               @focus="focus"
               @blur="blur">
    </form>
</template>

<script>
export default {
  name: 'AInputText',
  props: {
    text: String,
  },
  methods: {
    focus() {
      document.getElementById('input').placeholder = '';
    },
    blur() {
      document.getElementById('input').placeholder = this.text;
    },
  },
};
</script>

<style lang='stylus' scoped>
form{
  input {
    padding: 1rem;
    font-size: 17px;
    border: none;
    background: #fff;
    width: 90%;
  }
  width: 100%;
}
form:after {
  content: "";
  clear: both;
  border: none;
}
input:focus{
    outline: none;
}
</style>
