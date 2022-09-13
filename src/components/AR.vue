<script setup>
import { ref } from 'vue'
defineProps({
  msg: String
})


const count = ref(0)
</script>

<template>
   <!--图像加载前显示加载中...-->
      <!--a-scene会创建一个AR环境-->
      <a-scene embedded arjs="debugUIEnabled:false" vr-mode-ui="enabled:false">
          <!--a-marker是在相机中想要识别模型的标记-->
          <a-marker preset="hiro">
              <a-entity
              position="0 0.5 0"
              scale="1.5 1.5 1.5"
              rotation="0 0 0"
              gltf-model="/static/gltf/naruto/scene.gltf"
              ></a-entity>
          </a-marker>
          <a-marker preset='custom' type='pattern' url='/static/pattern/A.patt'>
            <a-entity
            position="0 0.5 0"
            scale="0.05 0.05 0.05"
            rotation="45 90 0"
            gltf-model="/static/gltf/bucket/scene.gltf"
            ></a-entity>
        </a-marker>
        <a-entity camera></a-entity>
      </a-scene>
</template>
