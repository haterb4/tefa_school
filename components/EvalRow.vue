<template>
    <div class="w-full h-[100px] rounded-[12px] flex justify-between items-center bg-cyan-50">
        <div class="w-[20%] h-full flex justify-center items-center">
            <div class="flex items-center gap-4">
                <div class="w-[65px] h-[65px] rounded-full bg-[#00A7DA] flex justify-center items-center">
                    <div class="progress-bar">
                        <progress class="progress-1" value="80" min="0" max="100" style="visibility:hidden;height:0;width:0;">75%</progress>
                    </div>
                </div>
                <div>
                    <h2 class="text-xl font-bold">Evaluation 1</h2>
                </div>
            </div>
        </div>
        <div class="w-[20%] h-full flex justify-center items-center">
            <div class="flex justify-center items-center gap-4">
                <font-awesome-icon :icon="['fas', 'file']" />
                <nuxt-link to="/empty">View Correction</nuxt-link>
            </div>
        </div>
        <div class="w-[20%] h-full flex justify-center items-center">
            <div class="flex justify-center items-center gap-4">
                <font-awesome-icon :icon="['fas', 'edit']" />
                <nuxt-link to="/empty">Retake Exam</nuxt-link>
            </div>
        </div>
        <div class="w-[20%] h-full flex justify-center items-center">
            <div class="flex justify-center items-center gap-4">
                <font-awesome-icon :icon="['fas', 'angles-up']" />
                <nuxt-link to="/empty">Upgrade</nuxt-link>
            </div>
        </div>
        <div class="w-[20%] h-full flex justify-center items-center">
            <div class="flex justify-center items-center gap-4">
                <font-awesome-icon :icon="['fas', 'chart-simple']" />
                <nuxt-link to="/empty">Last Result</nuxt-link>
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>

</script>

<style lang="css" scoped>
@property --progress-value {
  syntax: "<integer>";
  initial-value: 0;
  inherits: false;
}

@keyframes progress {
 to { --progress-value: 75; }
}

.progress-bar {
  display: flex;
  justify-content: center;
  align-items: center;

  width: 60px;
  height: 60px;
  border-radius: 50%;
  background: 
    radial-gradient(closest-side, #00A7DA 79%, transparent 80% 100%),
    conic-gradient(white calc(var(--progress-value) * 1%), #00A7DA 0);
  animation: progress 2s 1 forwards;
}

.progress-bar::before {
  counter-reset: percentage var(--progress-value);
  content: counter(percentage) '%';
  animation: progress 2s 1 forwards;
}
</style>