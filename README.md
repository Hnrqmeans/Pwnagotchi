🐧 Pwnagotchi Project

A self-learning Wi-Fi AI companion that evolves with you

Table of Contents Overview Features Hardware Components Configuration Setup Guide Contributing License & Acknowledgments
Overview 🇺🇸 English Pwnagotchi is an open-source project that creates an AI-powered companion for Wi-Fi security analysis. This self-learning tool improves its Wi-Fi handshake capture performance over time through reinforcement learning. My implementation runs on a Raspberry Pi Zero W with a Waveshare 2.13" e-Paper HAT (Rev2.1 V4) display and is powered by UPS-Lite v1.3 for portable operation.

🇧🇷 Português O Pwnagotchi é um projeto de código aberto que cria um companheiro com IA para análise de segurança Wi-Fi. Esta ferramenta de autoaprendizagem melhora seu desempenho na captura de handshakes Wi-Fi ao longo do tempo através de aprendizado por reforço. Minha implementação executa em um Raspberry Pi Zero W com display Waveshare 2.13" e-Paper HAT (Rev2.1 V4) e é alimentada por UPS-Lite v1.3 para operação portátil.

Features AI-Powered Learning: Improves handshake capture strategies over time Passive Monitoring: Analyzes Wi-Fi networks without active connection e-Paper Display: Low-power display showing status and activity Portable Operation: UPS-Lite provides battery backup Grid Reporting: Optional data sharing with pwnagotchi grid Multi-language: Full Brazilian Portuguese support

Hardware Components Component Specification Purpose Raspberry Pi Zero W Main computing unit Display Waveshare 2.13" e-Paper HAT Rev2.1 V4 Status visualization Power Supply UPS-Lite v1.3 Battery backup & power management Storage MicroSD Card (16GB+ recommended) Operating system & data

Initial Configuration

main.name = "pwnagotchi"
main.lang = "pt-br"
main.whitelist = [
  "EXAMPLE_NETWORK",
  "ANOTHER_EXAMPLE_NETWORK",
  "fo:od:ba:be:fo:od",
  "fo:od:ba"
]

main.plugins.grid.enabled = true
main.plugins.grid.report = true
main.plugins.grid.exclude = [
  "YourHomeNetworkHere"
]

ui.display.enabled = true
ui.display.type = "waveshare_3"
ui.display.color = "black"
