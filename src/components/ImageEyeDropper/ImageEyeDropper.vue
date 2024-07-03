<script setup lang="ts"></script>

<template>
    <div
        class="flex max-h-[479px] w-[327px] flex-col items-start rounded-md bg-[#1c1c1c] p-[10px_16px_16px_16px] shadow-[4px_4px_4px_0_rgba(0,0,0,0.25)]"
    >
        <div
            class="text-[12px] font-normal not-italic text-[rgba(255,255,255,0.8)]"
        >
            取色参考图，直接点击下方图片进行取色
        </div>
        <div
            class="mb-[18px] mt-[14px] cursor-pointer rounded border border-solid border-[rgba(255,255,255,0.22)]"
        >
            <!-- <UploadReference
                class="flex flex-row items-center justify-center"
                @reference-loaded="handleReferenceLoaded"
            > -->
            <div
                class="flex h-[32px] w-[186px] flex-row items-center justify-center gap-[10px]"
            >
                <!-- <Svg
                        class="reUpload-btn-icon"
                        :name="Svgs.RecolorEyeDropperUpload"
                    ></Svg> -->
                <div
                    class="text-[12px] font-semibold not-italic text-[rgba(255,255,255,0.9)]"
                >
                    重新上传参考图
                </div>
            </div>
            <!-- </UploadReference> -->
        </div>
        <div ref="imageWindowRef" class="relative self-center rounded-md">
            <div
                id="canvasWrapper"
                ref="canvasWrapperRef"
                class="absolute left-1/2 top-1/2 box-border origin-[0_0] cursor-none"
                :style="{ transform: `translate(-50%,-50%)` }"
            ></div>
        </div>
    </div>
</template>

<style scoped lang="scss"></style>
