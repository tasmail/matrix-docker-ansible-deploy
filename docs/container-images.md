# Container images used by the playbook

This page summarizes the container ([Docker](https://www.docker.com/)) images used by the playbook when setting up your server.

We try to stick to official images (provided by their respective projects) as much as possible.


## Container images used by default

These services are enabled and used by default, but you can turn them off, if you wish.

- [element-hq/synapse](https://ghcr.io/element-hq/synapse) - a fork of [matrixdotorg/synapse](https://github.com/matrix-org/synapse) Matrix homeserver

- [coturn/coturn](https://hub.docker.com/r/coturn/coturn/) - the [Coturn](https://github.com/coturn/coturn) STUN/TURN server (optional)

- [vectorim/element-web](https://hub.docker.com/r/vectorim/element-web/) - the [Element](https://element.io/) web client (optional)

- [postgres](https://hub.docker.com/_/postgres/) - the [Postgres](https://www.postgresql.org/) database server (optional)

- [devture/exim-relay](https://hub.docker.com/r/devture/exim-relay/) - the [Exim](https://www.exim.org/) email server (optional)

- [Traefik](https://hub.docker.com/_/traefik/) - the [Traefik](https://traefik.io/) web server (optional)

- [certbot/certbot](https://hub.docker.com/r/certbot/certbot/) - the [certbot](https://certbot.eff.org/) tool for obtaining SSL certificates from [Let's Encrypt](https://letsencrypt.org/) (optional)


## Optional other container images we may use

These services are not part of our default installation, but can be enabled by [configuring the playbook](configuring-playbook.md) (either before the initial installation or any time later):

- [ma1uta/ma1sd](https://hub.docker.com/r/ma1uta/ma1sd/) - the [ma1sd](https://github.com/ma1uta/ma1sd) Matrix Identity server (optional)

- [matrixconduit/matrix-conduit](https://hub.docker.com/r/matrixconduit/matrix-conduit) - the [Conduit](https://conduit.rs) Matrix homeserver (optional)

- [matrixdotorg/dendrite-monolith](https://hub.docker.com/r/matrixdotorg/dendrite-monolith/) - the [Dendrite](https://github.com/matrix-org/dendrite) Matrix homeserver (optional)

- [element-hq/hydrogen-web](https://ghcr.io/element-hq/hydrogen-web) - the [Hydrogen](https://github.com/element-hq/hydrogen-web) Matrix web client (optional)

- [ajbura/cinny](https://hub.docker.com/r/ajbura/cinny) - the [Cinny](https://github.com/ajbura/cinny) Matrix web client (optional)

- [etke.cc/schildichat-web](https://ghcr.io/etkecc/schildichat-web) - the [SchildiChat](https://github.com/SchildiChat/schildichat-desktop) Matrix web client (optional)

- [activism.international/matrix_ldap_registration_proxy](https://gitlab.com/activism.international/matrix_ldap_registration_proxy/container_registry) - the [matrix-ldap-registration-proxy](https://gitlab.com/activism.international/matrix_ldap_registration_proxy) for handling Matrix registration requests and forwards them to LDAP (optional)

- [ewoutp/goofys](https://hub.docker.com/r/ewoutp/goofys/) - the [Goofys](https://github.com/kahing/goofys) Amazon [S3](https://aws.amazon.com/s3/) file-system-mounting program (optional)

- [t2bot/matrix-media-repo](https://ghcr.io/t2bot/matrix-media-repo) - the [matrix-media-repo](https://docs.t2bot.io/matrix-media-repo/) highly customizable multi-domain media repository (optional)

- [etherpad/etherpad](https://hub.docker.com/r/etherpad/etherpad/) - the [Etherpad](https://etherpad.org) realtime collaborative text editor that can be used in a Jitsi audio/video call or integrated as a widget into Matrix chat rooms via the Dimension integration manager (optional)

- [devture/email2matrix](https://hub.docker.com/r/devture/email2matrix/) - the [Email2Matrix](https://github.com/devture/email2matrix) email server, which can relay email messages to Matrix rooms (optional)

- [devture/matrix-corporal](https://hub.docker.com/r/devture/matrix-corporal/) - [Matrix Corporal](https://github.com/devture/matrix-corporal): reconciliator and gateway for a managed Matrix server (optional)

- [zeratax/matrix-registration](https://hub.docker.com/r/devture/zeratax-matrix-registration/) - [matrix-registration](https://github.com/ZerataX/matrix-registration): a simple python application to have a token based Matrix registration (optional)

- [matrixdotorg/matrix-user-verification-service](https://hub.docker.com/r/matrixdotorg/matrix-user-verification-service) - [Matrix User Verification Service](https://github.com/matrix-org/matrix-user-verification-service) for verifying details of a user based on an Open ID token (optional)

- [mautrix/discord](https://mau.dev/mautrix/discord/container_registry) - the [mautrix-discord](https://github.com/mautrix/discord) bridge to [Discord](https://discord.com/) (optional)

- [mautrix/slack](https://mau.dev/mautrix/slack/container_registry) - the [mautrix-slack](https://github.com/mautrix/slack) bridge to [Slack](https://slack.com/) (optional)

- [mautrix/telegram](https://mau.dev/mautrix/telegram/container_registry) - the [mautrix-telegram](https://github.com/mautrix/telegram) bridge to [Telegram](https://telegram.org/) (optional)

- [mautrix/gmessages](https://mau.dev/mautrix/gmessages/container_registry) - the [mautrix-gmessages](https://github.com/mautrix/gmessages) bridge to [Google Messages](https://messages.google.com/) (optional)

- [mautrix/whatsapp](https://mau.dev/mautrix/whatsapp/container_registry) - the [mautrix-whatsapp](https://github.com/mautrix/whatsapp) bridge to [Whatsapp](https://www.whatsapp.com/) (optional)

- [mautrix/wsproxy](https://mau.dev/mautrix/wsproxy/container_registry) - the [mautrix-wsproxy](https://github.com/mautrix/wsproxy) bridge to Android SMS or Apple iMessage (optional)

- [mautrix/twitter](https://mau.dev/mautrix/twitter/container_registry) - the [mautrix-twitter](https://github.com/mautrix/twitter) bridge to [Twitter](https://twitter.com/) (optional)

- [mautrix/googlechat](https://mau.dev/mautrix/googlechat/container_registry) - the [mautrix-googlechat](https://github.com/mautrix/googlechat) bridge to [Google Chat](https://en.wikipedia.org/wiki/Google_Chat) (optional)

- [mautrix/meta](https://mau.dev/mautrix/meta/container_registry) - the [mautrix-meta](https://github.com/mautrix/meta) bridge to [Messenger](https://messenger.com/) and [Instagram](https://instagram.com/) (optional)

- [mautrix/signal](https://mau.dev/mautrix/signal/container_registry) - the [mautrix-signal](https://github.com/mautrix/signal) bridge to [Signal](https://www.signal.org/) (optional)

- [beeper/linkedin](https://ghcr.io/beeper/linkedin) - the [beeper-linkedin](https://github.com/beeper/linkedin) bridge to [LinkedIn](https://www.linkedin.com/) Messaging (optional)

- [matrixdotorg/matrix-appservice-irc](https://hub.docker.com/r/matrixdotorg/matrix-appservice-irc) - the [matrix-appservice-irc](https://github.com/matrix-org/matrix-appservice-irc) bridge to [IRC](https://wikipedia.org/wiki/Internet_Relay_Chat) (optional)

- [matrix-org/matrix-appservice-discord](https://ghcr.io/matrix-org/matrix-appservice-discord) - the [matrix-appservice-discord](https://github.com/matrix-org/matrix-appservice-discord) bridge to [Discord](https://discordapp.com/) (optional)

- [matrixdotorg/matrix-appservice-slack](https://hub.docker.com/r/matrixdotorg/matrix-appservice-slack) - the [matrix-appservice-slack](https://github.com/matrix-org/matrix-appservice-slack) bridge to [Slack](https://slack.com/) (optional)

- [halfshot/matrix-hookshot](https://hub.docker.com/r/halfshot/matrix-hookshot) - the [matrix-hookshot](https://github.com/matrix-org/matrix-hookshot) Bridge for generic webhooks and multiple project management services (optional)

- [folivonet/matrix-sms-bridge](https://hub.docker.com/repository/docker/folivonet/matrix-sms-bridge) - the [matrix-sms-bridge](https://github.com/benkuly/matrix-sms-bridge) (optional)

- [lxduo/matrix-wechat](https://hub.docker.com/r/lxduo/matrix-wechat) - the [matrix-wechat](https://github.com/duo/matrix-wechat) bridge to WeChat (optional)

- [hif1/heisenbridge](https://hub.docker.com/r/hif1/heisenbridge) - the [Heisenbridge](https://github.com/hifi/heisenbridge) bouncer-style bridge to [IRC](https://wikipedia.org/wiki/Internet_Relay_Chat) (optional)

- [nodefyme/go-skype-bridge](https://hub.docker.com/r/nodefyme/go-skype-bridge) - the [go-skype-bridge](https://github.com/kelaresg/go-skype-bridge) to [Skype](https://www.skype.com/) (optional)

- [mx-puppet/discord/mx-puppet-discord](https://gitlab.com/mx-puppet/discord/mx-puppet-discord/container_registry) - the [mx-puppet-discord](https://gitlab.com/mx-puppet/discord/mx-puppet-discord) bridge to [Discord](https://discordapp.com) (optional)

- [mx-puppet/slack/mx-puppet-slack](https://gitlab.com/mx-puppet/slack/mx-puppet-slack/container_registry) - the [mx-puppet-slack](https://gitlab.com/mx-puppet/slack/mx-puppet-slack) bridge to [Slack](https://slack.com) (optional)

- [sorunome/mx-puppet-instagram](https://hub.docker.com/r/sorunome/mx-puppet-instagram) - the [mx-puppet-instagram](https://github.com/Sorunome/mx-puppet-instagram) bridge to [Instagram](https://www.instagram.com) (optional)

- [sorunome/mx-puppet-twitter](https://hub.docker.com/r/sorunome/mx-puppet-twitter) - the [mx-puppet-twitter](https://github.com/Sorunome/mx-puppet-twitter) bridge to [Twitter](https://twitter.com) (optional)

- [xangelix/mx-puppet-groupme](https://hub.docker.com/r/xangelix/mx-puppet-groupme) - the [mx-puppet-groupme](https://gitlab.com/xangelix-pub/matrix/mx-puppet-groupme) bridge to [GroupMe](https://groupme.com/) (optional)

- [icewind1991/mx-puppet-steam](https://hub.docker.com/r/icewind1991/mx-puppet-steam) - the [mx-puppet-steam](https://github.com/icewind1991/mx-puppet-steam) bridge to [Steam](https://steampowered.com) (optional)

- [linuxserver/ddclient](https://hub.docker.com/r/linuxserver/ddclient) - [ddclient](https://github.com/linuxserver/docker-ddclient) used to update dynamic DNS entries for accounts on Dynamic DNS Network Service Provider (optional)

- [jitsi/web](https://hub.docker.com/r/jitsi/web) - the [Jitsi](https://jitsi.org/) web UI (optional)

- [jitsi/jicofo](https://hub.docker.com/r/jitsi/jicofo) - the [Jitsi](https://jitsi.org/) Focus component (optional)

- [jitsi/prosody](https://hub.docker.com/r/jitsi/prosody) - the [Jitsi](https://jitsi.org/) Prosody XMPP server component (optional)

- [jitsi/jvb](https://hub.docker.com/r/jitsi/jvb) - the [Jitsi](https://jitsi.org/) Video Bridge component (optional)

- [etke.cc/baibot](https://ghcr.io/etkecc/baibot) - the [baibot](https://github.com/etkecc/baibot) for accessing [Large Language Models](https://en.wikipedia.org/wiki/Large_language_model) (optional)

- [anoa/matrix-reminder-bot](https://hub.docker.com/r/anoa/matrix-reminder-bot) - the [matrix-reminder-bot](https://github.com/anoadragon453/matrix-reminder-bot) bot for one-off & recurring reminders and alarms (optional)

- [moanos/matrix-registration-bot/](https://hub.docker.com/r/moanos/matrix-registration-bot/) - the [matrix-registration-bot](https://github.com/moan0s/matrix-registration-bot) bot (manage registration tokens for invitations to the server) (optional)

- [dock.mau.dev/maubot/maubot](https://mau.dev/maubot/maubot/container_registry) - the [maubot](https://github.com/maubot/maubot) bot (a plugin-based Matrix bot system) (optional)

- [etke.cc/honoroit](https://github.com/etkecc/honoroit/container_registry) - the [Honoroit](https://github.com/etkecc/honoroit) helpdesk bot (optional)

- [etke.cc/postmoogle](https://github.com/etkecc/postmoogle/container_registry) - the [Postmoogle](https://github.com/etkecc/postmoogle) email bridge bot (optional)

- [matrixdotorg/mjolnir](https://hub.docker.com/r/matrixdotorg/mjolnir) - the [Mjolnir](https://github.com/matrix-org/mjolnir) moderation bot (optional)

- [gnuxie/draupnir](https://hub.docker.com/r/gnuxie/draupnir) - the [Draupnir](https://github.com/the-draupnir-project/Draupnir/) moderation bot (optional)

- [etke.cc/buscarron](https://ghcr.io/etkecc/buscarron) - the [Buscarron](https://github.com/etkecc/buscarron) bot for web forms (HTTP POST) (optional)

- [metio/matrix-alertmanager-receiver](https://hub.docker.com/r/metio/matrix-alertmanager-receiver) - the [matrix-alertmanager-receiver](https://github.com/metio/matrix-alertmanager-receiver) client for Prometheus' [Alertmanager](https://prometheus.io/docs/alerting/latest/alertmanager/) (optional)

- [element-hq/matrix-authentication-service](https://ghcr.io/element-hq/matrix-authentication-service) - [matrix-authentication-service](https://github.com/element-hq/matrix-authentication-service) (MAS) OAuth 2.0 and OpenID Provider server (optional)

- [etke.cc/synapse-admin](https://ghcr.io/etkecc/synapse-admin) - the [etkecc/synapse-admin](https://github.com/etkecc/synapse-admin) (a [feature-rich](https://github.com/etkecc/synapse-admin#fork-differences) fork of [Awesome-Technologies/synapse-admin](https://github.com/Awesome-Technologies/synapse-admin) web UI tool for administrating users and rooms on your Matrix server (optional)

- [matrix-org/rageshake](https://ghcr.io/matrix-org/rageshake) - the [rageshake](https://github.com/matrix-org/rageshake) bug report server (optional)

- [prom/prometheus](https://hub.docker.com/r/prom/prometheus/) - [Prometheus](https://github.com/prometheus/prometheus/) is a systems and service monitoring system

- [prom/node-exporter](https://hub.docker.com/r/prom/node-exporter/) - [Prometheus Node Exporter](https://github.com/prometheus/node_exporter/) is an addon for Prometheus that gathers standard system metrics

- [martin-helmich/prometheus-nginxlog-exporter/exporter](https://ghcr.io/martin-helmich/prometheus-nginxlog-exporter/exporter) - [NGINX-to-Prometheus log file exporter](https://github.com/martin-helmich/prometheus-nginxlog-exporter/) is an addon for Prometheus that gathers access logs from various nginx reverse-proxies (optional)

- [grafana/grafana](https://hub.docker.com/r/grafana/grafana/) - [Grafana](https://github.com/grafana/grafana/) is a graphing tool that works well with the above two images. Our playbook also adds two dashboards for [Synapse](https://github.com/element-hq/synapse/tree/master/contrib/grafana) and  [Node Exporter](https://github.com/rfrail3/grafana-dashboards)

- [matrixdotorg/sygnal](https://hub.docker.com/r/matrixdotorg/sygnal/) - [Sygnal](https://github.com/matrix-org/sygnal) is a reference Push Gateway for Matrix

- [binwiederhier/ntfy](https://hub.docker.com/r/binwiederhier/ntfy/) - [ntfy](https://ntfy.sh/) is a self-hosted, UnifiedPush-compatible push notifications server

- [matrix-org/sliding-sync](https://ghcr.io/matrix-org/sliding-sync) - the [Sliding Sync](https://github.com/matrix-org/sliding-sync) proxy (optional)

- [etke.cc/rust-synapse-compress-state](https://gitlab.com/etke.cc/rust-synapse-compress-state/container_registry) - [synapse-auto-compressor](https://github.com/matrix-org/rust-synapse-compress-state/#automated-tool-synapse_auto_compressor) for automatic compression of Synapse's `state_groups` database table (optional)

- [cactuscomments/cactus-appservice](https://hub.docker.com/r/cactuscomments/cactus-appservice/) and [joseluisq/static-web-server](https://hub.docker.com/r/joseluisq/static-web-server) - [Cactus Comments](https://cactus.chat) a federated comment system built on Matrix

- [matrixdotorg/pantalaimon](https://hub.docker.com/r/matrixdotorg/pantalaimon) - the [pantalaimon](https://github.com/matrix-org/pantalaimon) E2EE aware proxy daemon (optional)

## Container images of deprecated / unmaintained services

The list of the deprecated or unmaintained services is available [here](configuring-playbook.md#deprecated--unmaintained--removed-services).

- [turt2live/matrix-appservice-webhooks](https://hub.docker.com/r/turt2live/matrix-appservice-webhooks) - the [Appservice Webhooks](https://github.com/turt2live/matrix-appservice-webhooks) bridge (optional)

- [turt2live/matrix-dimension](https://hub.docker.com/r/turt2live/matrix-dimension) - the [Dimension](https://dimension.t2bot.io/) integration manager (optional)

- [matrixdotorg/go-neb](https://hub.docker.com/r/matrixdotorg/go-neb) - the [Go-NEB](https://github.com/matrix-org/go-neb) bot (optional)

- [matrixgpt/matrix-chatgpt-bot](https://ghcr.io/matrixgpt/matrix-chatgpt-bot) - the [matrix-chatgpt-bot](https://github.com/matrixgpt/matrix-chatgpt-bot) for accessing ChatGPT via your favourite Matrix client (optional)

- [mautrix/facebook](https://mau.dev/mautrix/facebook/container_registry) - the [mautrix-facebook](https://github.com/mautrix/facebook) bridge to [Facebook](https://facebook.com/) (optional)

- [mautrix/hangouts](https://mau.dev/mautrix/hangouts/container_registry) - the [mautrix-hangouts](https://github.com/mautrix/hangouts) bridge to [Google Hangouts](https://en.wikipedia.org/wiki/Google_Hangouts) (optional)

- [mautrix/instagram](https://mau.dev/mautrix/instagram/container_registry) - the [mautrix-instagram](https://github.com/mautrix/instagram) bridge to [Instagram](https://instagram.com/) (optional)
