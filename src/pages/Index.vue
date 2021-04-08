<template>
  <q-page class="flex flex-center">
    <q-btn @click="callHaptics()">
      haptic test
    </q-btn>
  </q-page>
</template>

<script>
import { Haptics, ImpactStyle, NotificationType } from '@capacitor/haptics';

export default {
  name: 'PageIndex',

  methods:  {
    callHaptics() { 
      Haptics.impact({ style: NotificationType.SUCCESS });
    }
  }
}
</script>
