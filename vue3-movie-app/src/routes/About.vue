<template>
    <div class="about">
        <div class="name">{{ name }}</div>
        <div> {{email}} </div>
        <div> {{blog}} </div>
        
    </div>
</template>

<script>
import { mapState } from 'vuex'

export default {
    computed: {
        ...mapState('about', [            
            'name',
            'email',
            'blog'
        ])        
    }
}
</script>

<style lang="scss" scoped>


.about {
    text-align: center;
    
    .name {
        margin-top: 40px;
        margin-bottom: 20px;
        padding: 30px;
        font-size: 40px;
        font-family: "Oswald", sans-serif;
        
    }
}
</style>
