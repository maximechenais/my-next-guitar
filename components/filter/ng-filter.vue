<template>
    <div class="filter-container">
        <div class="filter-title">
            <h1>{{ filterTitle }}</h1>
            <img src="@/assets/icons/filter-icon.svg" class="filter-image" alt="filter-image">
        </div>
        <div class="inputs-container">
            <div class="brand-list">
                <select class="select-brand">
                    <option v-for="brand in brands">{{ brand.name }}</option>
                </select>
            </div>
            <div class="color-list">
                <select class="select-color">
                    <option v-for="color in guitarColor">{{ color.color }}</option>
                </select>
            </div>
        </div>
        <div class="average-range">
            <input type="range">
        </div>

    </div>
</template>

<script>
    import inputSelect from '@/components/input/input-select'

    export default {
        name: 'ngFilter',

        components: {
            inputSelect,
        },

        data() {
            return {
                filterTitle: 'Search by filters',
                brands: [{
                    name: 'guitar 1'
                }, {
                    name: 'guitar 2'
                }, {
                    name: 'guitar 3'
                }, {
                    name: 'guitar 4'
                }, ],
                guitarColor: [{
                    color: 'white'
                }, {
                    color: 'black'
                }, {
                    color: 'yellow'
                }, {
                    color: 'red'
                }, ]
            }
        }
    }
</script>

<style scoped>
    .filter-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 334px;
        height: 350px;
        background: #FFFFFF;
        border: 1px solid #CFCFCF;
        box-shadow: 0px 0px 12px 2px rgba(86, 197, 204, 0.25);
        border-radius: 10px;
    }
    
    .filter-title {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: flex-start;
        margin: 20px 0 20px 0;
        width: 300px;
    }
    
    .filter-title h1 {
        color: #222323;
        font-size: 18px;
        font-weight: 600;
        margin-right: 5px;
    }
    
    .filter-image {
        height: 25px;
        width: 25px;
    }
    
    .inputs-container {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: space-evenly;
        width: 300px;
        height: 151px;
    }
    
    select {
        width: 300px;
        height: 58px;
        border: 1px solid #CFCFCF;
        box-shadow: inset 0px 4px 4px rgba(86, 197, 204, 0.25);
        border-radius: 10px;
        outline: none;
        margin-bottom: 10px;
        padding: 10px;
        font-size: 14px;
        color: 555454;
    }
</style>