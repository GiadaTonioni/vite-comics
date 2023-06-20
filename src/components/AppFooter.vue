<script>
export default {

}
</script>
<template>
    <div>
        <footer>
            <div class="container">
                <div class="row">
                    <div class="col">BUTTON</div>
                    <div class="col">Follow loghi</div>
                </div>
            </div>
        </footer>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variables' as*;

.row {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.col {
    background-color: pink;
    height: 120px;
    width: 700px;
}
</style>