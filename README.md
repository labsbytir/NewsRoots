# NewsRoots

NewsRoots is the monorepo for the newsroom stack. It brings the NewsRock application, Newspack Bedrock site, NewsWoo plugin, NewsDesk theme, and NewsRockQA project together in one repository.

## Projects

| Path | Project |
| --- | --- |
| Repository root | NewsRock application and shared configuration |
| [`newspack-bedrock/`](newspack-bedrock/) | Newspack on Roots Bedrock and Acorn |
| [`newswoo/`](newswoo/) | WooCommerce fork for newsroom subscriptions and paywall |
| [`newsdesk/`](newsdesk/) | Newspack theme for Bedrock and Sage |
| [`newsrockqa/`](newsrockqa/) | NewsRock QA project |

Each product keeps its own dependency and build configuration. Run its commands from that product's directory.

## Newspack Bedrock

```bash
cd newspack-bedrock
cp .env.example .env
composer install
```

The web root is `newspack-bedrock/web/`. Plugin sources are in `newspack-bedrock/packages/` and install into `web/app/plugins/` through Composer.

## NewsWoo

See [`newswoo/README.md`](newswoo/README.md) for setup and development details.

## NewsDesk

See [`newsdesk/README.md`](newsdesk/README.md) for project details.

## CI

GitHub Actions validates and tests the Newspack Bedrock and NewsWoo projects when their files change.

## License

GPL-2.0-or-later for the newsroom stack and WordPress plugins. Roots Bedrock and Acorn are MIT licensed.
