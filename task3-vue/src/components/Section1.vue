
<template>
 
    
            <div class="col-lg-6 col-xxl-4 mb-5">
                <div class="card bg-light border-0 h-100">
                    <div class="card-body text-center p-4 flex-column p-lg-5">
                        <div class="feature bg-primary bg-gradient text-white rounded-3 mb-4 mt-n4"><i :class="person.urlimg"></i></div>
                        <h2 class="fs-4 fw-bold">{{ person.title }}</h2>
                        <p class="mb-0">{{ person.disc }}</p>
                    </div>
                </div>
            </div>
       
</template>
<script>
export default {
    props: ["person"]
};
</script>
<style>
.card-body{
    display: flex;
    align-items: center;
    justify-content: center;
}
.feature{
    width: 100px;
    height: 70px;
    display: flex;
    align-items: center;
    justify-content: center;
}
i{
    font-size: 40px;
}
</style>
