<template>
  <div class="search">
    <form id="search-form">
      <input type="search" placeholder="Search">

    </form>
  </div>
</template>

<script>
import SearchSvg from '@/assets/icons/search.svg';
import AInputText from '@/components/atoms/a-input-text';

export default {
  name: 'MSearch',
  components: {
    AInputText,
    SearchSvg,
  },
};
</script>

<style lang='stylus' scoped>

input {
	outline: none;
}
input[type=search] {
	-webkit-appearance: textfield;
	-webkit-box-sizing: content-box;
	font-family: inherit;
  font-size: 14px;
}
input::-webkit-search-decoration,
input::-webkit-search-cancel-button {
	display: none; 
}


input[type=search] {
	background: #fff url(https://static.tumblr.com/ftv85bp/MIXmud4tx/search-icon.png) no-repeat 9px center;
	border: solid 1px #fff;
	padding: 9px 10px 9px 32px;
	width: 55px;

  -webkit-transition: all .5s;
	-moz-transition: all .5s;
	transition: all .5s;
}

input:-moz-placeholder {
	color: #999;
}
input::-webkit-input-placeholder {
	color: #999;
}

input[type=search] {
	width: 15px;
	padding-left: 10px;
	color: transparent;
	cursor: pointer;
}
input[type=search]:hover {
	background-color: #fff;
}
input[type=search]:focus {
	width: 170px;
	padding-left: 32px;
	color: #ccc;
	background-color: #fff;
	cursor: auto;
  border-color: rgba(0, 0, 0, 0.15);
}
input:-moz-placeholder {
	color: transparent;
}
input::-webkit-input-placeholder {
	color: transparent;
}

</style>
