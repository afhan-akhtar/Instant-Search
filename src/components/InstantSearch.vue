<template>
    <div>
        <h1>Instant Search App</h1>
        <input type="text" v-model="searchTerm" placeholder="Search..." />
        <ul class="centered-list">
            <li v-for="result in filteredResults" :key="result.id">{{ result.title }}</li>
        </ul>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            searchTerm: "",
            results: [
                { id: 1, title: "Apple" },
                { id: 2, title: "Blackberry" },
                { id: 3, title: "Computer" },
                { id: 4, title: "Date" },
                { id: 5, title: "England" },
            ],
        };
    },
    computed: {
        filteredResults() {
            return this.results.filter((result) =>
                result.title.toLowerCase().includes(this.searchTerm.toLowerCase())
            );
        },
    },
};
</script>