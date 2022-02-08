<script setup>
import { WalletMultiButton, WalletModalProvider } from '@solana/wallet-adapter-vue-ui';

</script>

<template>
    <wallet-modal-provider>
      <wallet-multi-button></wallet-multi-button>
    </wallet-modal-provider>
</template>