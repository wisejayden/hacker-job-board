<template>
    <footer>
        <p>{{copyright}}</p>
    </footer>
</template>

<script>
export default {
    data() {
        return {
            copyright: 'Open Source made available by Jayden Wise'
        }
    }
}
</script>

<style scoped>
    footer {
        background: #222;
        padding: 6px;
    }
    p {
        color: #fe6501;
        text-align: center;
    }
</style>
