<script setup>
import ChildComponent from './components/ChildComponent.vue';
import { getPhantomWallet, getSolflareWallet } from "@solana/wallet-adapter-wallets";
import { WalletProvider } from "@solana/wallet-adapter-vue";

const wallets = [
  getPhantomWallet(),
  getSolflareWallet(),
]
</script>

<template>
  <wallet-provider :wallets="wallets" auto-connect>
    <child-component></child-component>
  </wallet-provider>
</template>