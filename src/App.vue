<script setup>
import {ref} from 'vue'
const page = ref(1)
</script>

<template>
    <div class="container pt-5">
        <div class="row">
            <div class="col-md-3">
                <div class="tab-list">
                    <div :class="page==1?'active':''" class="item" @click="page=1">Home</div>
                    <div :class="page==2?'active':''" class="item" @click="page=2">About</div>
                    <div :class="page==3?'active':''" class="item" @click="page=3">Contact</div>
                </div>
            </div>
            <div class="col-md-9">
                <div class="tab-content">
                    <div class="item" v-show="page==1">
                        <h3>Home Page</h3>
                        <p>
                            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Molestias fuga dolorum dolores accusantium a ex illo modi? Maxime tenetur officia odio, reprehenderit excepturi, beatae temporibus molestias nisi optio delectus officiis veritatis quod! Adipisci blanditiis officia vel distinctio. Libero sed aperiam numquam fugiat expedita doloremque. Esse molestiae dolor sapiente saepe nihil.
                        </p>
                    </div>
                    <div class="item" v-show="page==2">
                        <h3>About Page</h3>
                        <p>
                            Omnis libero, id reiciendis aliquam, facilis dolores veritatis eligendi nihil fuga quod illo. Inventore voluptatem ipsa quas minima odio, obcaecati blanditiis omnis voluptas aspernatur error ipsum tenetur fuga exercitationem architecto laudantium quis. Explicabo neque qui quos totam facere odio itaque quibusdam doloremque molestias sit, voluptatum earum, dignissimos, cumque quae.
                        </p>
                    </div>
                    <div class="item" v-show="page==3">
                        <h3>Contact Page</h3>
                        <p>
                            Reiciendis voluptatum facilis expedita harum laudantium, dignissimos sit quos corporis consequatur dolorum voluptates temporibus est, aliquid distinctio non in incidunt eos eaque praesentium libero cumque. Mollitia, vitae dolor enim doloribus sunt dolorum numquam quasi ipsam deleniti nostrum voluptate quos sequi. Laborum delectus enim voluptatum, sed totam assumenda ut iure obcaecati quibusdam eligendi harum quam facilis corrupti ad minima culpa veniam reiciendis, laboriosam facere soluta, consequatur similique quis?
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>