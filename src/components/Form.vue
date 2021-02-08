<template>
    <form @submit.prevent="search"
    action="" class="form-inline d-flex justify-content-center">
        <input type="text" placeholder="Search Pokemon" class="form-control" v-model="searchText">
        <input type="submit" value="Cerca" class="btn btn-primary ml-2">
    </form>
</template>
<script>
    export default {
        name: 'Form',
        data() {
            return {
                searchText: ''
            }
        },
        methods: {
            search() {
                this.$emit('newSearch', this.searchText);

            }
        }
    }
</script>
