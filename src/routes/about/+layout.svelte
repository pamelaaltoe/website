<script>
	import { base } from "$app/paths";

</script>
<div class="base">
    <div class="cornice"
    <slot/>
<div/>

<style>
.base{
    padding:20px
}

.cornice{
    border: 2px;
    solid: red;
    border-radius: 20px;
    padding: 20px;
}

</style>