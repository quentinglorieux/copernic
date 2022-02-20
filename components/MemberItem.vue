<template>
<div>
    <div  class="flex m-10 text-gray-400">
        <div>
            <div class=" text-gray-300 shadow-xs text-2xl mb-10"> 
                {{ memberData.firstname}} {{ memberData.lastname}} </div>
        {{ memberData.description }}
        </div>

        <nuxt-img class=" object-contain w-200 ml-10" :src="memberData.image" 
            width="200"
        />
    </div>
</div>
</template>

<script>
export default {
  props: {
      memberData: '',
  },

}
</script>

