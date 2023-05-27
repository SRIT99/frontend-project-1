<template>
    <div class="card" style="width: 18rem;">
            <img
              :src="data.url"
              class="card-img-top"
              alt="..."
            />
            <div class="card-body">
              <h5 class="card-title">{{ data.title }}</h5>
              <p class="card-text">Lorem ipsum dolor sit amet..</p>
              <a href="#" class="btn btn-primary">see more</a>
            </div>
     </div>
         
</template>
<script>
export default{
    name: "CardComponent",
    props:{
        data: {},
    },
};
</script>