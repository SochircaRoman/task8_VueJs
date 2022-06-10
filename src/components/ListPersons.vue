<template>
    <div class="wraper">
            <div class="element">
                <label for="name"><strong>Name:</strong></label>
                <span id="name"><i>{{ ` ${personArr.name}` }}</i></span>
            </div>
            <div class="element">
                <label for="phone"><strong>Phone:</strong> </label>
                <span id="phone"><i>{{ ` ${personArr.user}` }}</i></span>
            </div>
            <div class="element">
                <label for="email"><strong>Email:</strong></label>
                <span id="email"><i>{{ ` ${personArr.admin}` }}</i></span>
            </div>
        </div>
</template>

<script>
export default {
    data() {
        return {
            personsArr: [
                {name: "Name", user: "Sochirca Roman", admin: "Sochirca Roman"},
            ],
        }
    },
    methods: {
        
}
}
</script>

<style scoped>

.wraper{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items:flex-start;
    margin-top: 50px;
    margin-right: 50px;
}

.element {
    border: 1px solid #000;
    padding: 15px;
    width: 170px;
    cursor: pointer;
}

.element:hover {
  border: 3px solid aquamarine;
}


</style>