<template>
    <div class="mobile">
        <div class="flex items-center note">
            <div class="flex items-center justify-center note-img"> 
                <img src="../assets/notify.svg" alt="notification" width="18" height="18">
            </div>
            <span>Prank call was pulled off <b>AUTOMATICALLY</b> with our app!</span>
            <button>Try it now</button>
        </div>
        <VoicedBy/>
    </div>
</template>
<script>
    import VoicedBy from '@/components/VoicedBy.vue'
    export default {
        components: {
            VoicedBy
        }
    }
</script>
<style>
    .note {
        background: rgba(255, 165, 0, 0.2);
        padding: 10px 18px;
        margin-top: 15px;
        display: flex;
        align-items: center;
    }
    .note span {
        font-size: 12px;
        text-align: left;
        margin-left: 10px;
        width: 100%;
    }
    .note-img {
        background: #fff;
        border: 1px solid rgba(0, 0, 0, 0.05);
        border-radius: 8px;
        max-width: 36px;
        max-height: 36px;
        padding: 10px;
    }
    .note button {
        background: #2FDBD9;
        border: 1px solid rgba(47, 56, 78, 0.1);
        border-radius: 10px;
        color: #fff;
        min-width: 98px;
        margin-left: 5px;
        max-height: 36px;
    }
</style>
