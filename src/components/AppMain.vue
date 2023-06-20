<script>
export default {

}
</script>
<template>
    <div>
        <main>
            <div class="container">
                <div class="row">
                    <div class="col-list">
                        <div class="container">
                            <div class="row-list">
                                <div class="col-small">
                                    <h4>UNO</h4>
                                    <ul>
                                        <li>1</li>
                                    </ul>
                                </div>
                                <div class="col-small">
                                    <h4>DUE</h4>
                                    <ul>
                                        <li>2</li>
                                    </ul>
                                </div>
                                <div class="col-small">
                                    <h4>TRE</h4>
                                    <ul>
                                        <li>3</li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-back">
                        LOGONE
                    </div>
                </div>
            </div>
        </main>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as*;

.row {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.col-list {
    border: 1px solid black;
    height: 400px;
    width: 40%;
    background-color: aqua;
}

.col-back {
    border: 1px solid black;
    height: 400px;
    width: 50%;
    background-color: rgb(72, 0, 255);
}

.row-list {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
}

.col-small {
    height: 300px;
    width: 20%;
    background-color: beige;
}
</style>