<template>
    <div class="input-bg">
        <div class="videoImg">
            <!--        <img src="" alt="">-->
            <div>🤿</div>
        </div>

        <input type="text" class="inputMsg">

        <div class="flex input-content">
            <div>
                😀
            </div>
            <div>
                +
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "index"
}
</script>

<style>


.input-bg {
    background: white;
    display: flex;
    width: 100%;
}

.flex {
    display: flex;
}

.videoImg * {
    font-size: 24px;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;

}

.inputMsg {
    min-width: 70vw;
    background: #efefef;
    padding: 5px;
    padding-left: 20px;
    margin: 10px;
}

.input-content {
    justify-content: space-around;
    width: 100%;
    align-items: center;
    font-size: 22px;
}

input{
    outline: none;
}
</style>
