<template>
    <div class="parent">
        <span class="inject_span" v-for="item in items" :key="item[`title`]">

            <h1>{{ item[`title`] }}</h1>

            <p>{{ item[`price`] }}</p>

            <p>{{ item[`description`] }}</p>

            <img class="animated-gif" v-bind:src="item[`img_url`]">
        </span>
    </div>
</template>

<script>
export default {
    data() {
        return {
            items: [{


                title: `thunderfury`,

                price: `5 gold`,

                description: `thunderfury, blessed blade of the windseeker`,

                img_url: `https://www.hiveworkshop.com/data/ratory-images/216/216302-77a81ccc6c3d8e9e563a7b4582de8c70.gif`



            },



            {


                title: `thunderfury`,

                price: `5 gold`,

                description: `thunderfury, blessed blade of the windseeker`,

                img_url: `https://www.hiveworkshop.com/data/ratory-images/216/216302-77a81ccc6c3d8e9e563a7b4582de8c70.gif`



            },

            {


                title: `thunderfury`,

                price: `5 gold`,

                description: `thunderfury, blessed blade of the windseeker`,

                img_url: `https://www.hiveworkshop.com/data/ratory-images/216/216302-77a81ccc6c3d8e9e563a7b4582de8c70.gif`



            }

            ]
        }
    },
}
</script>

<style scoped>



.parent{


    display: grid;

    grid-template-rows: 1fr 1fr 1fr;

        justify-items: center;

    align-items: center;

    text-align: center;

}

.parent>.inject_span{
    display: grid;

    justify-items: center;

    align-items: center;

    text-align: center;

    background-color: #BEE3DB;

    grid-template-rows: 16vh 8vh 8vh 20vh;

    margin-top: 25px;

    margin-bottom: 25px;

    width: 80%;

}
img.animated-gif {

    width: 220px;


    height: auto;

}
</style>

