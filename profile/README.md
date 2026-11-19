<div align="center">
  <a href="https://calistar.io">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Calistar-io/.github/main/profile/logo-dark.svg" />
      <img src="https://raw.githubusercontent.com/Calistar-io/.github/main/profile/logo-light.svg" alt="Calistar" width="96" />
    </picture>
  </a>

# Calistar

**Privacy-first web and API analytics for Stellar ecosystem projects.**

[**Website**](https://calistar.io) · [**Documentation**](https://calistar.io/docs)

</div>

Calistar is a proposed open-source service that measures web and API usage across projects
building on Stellar, without collecting personal data. It answers the Stellar Community Fund RFP
*Web and API Analytics for Stellar Ecosystem Projects*.

1. **Web analytics**: one version-pinned script in the browser, processed by an unmodified
   release of [Umami](https://github.com/umami-software/umami). No cookies, no device storage,
   no stored IP addresses.
2. **API analytics**: OpenTelemetry metrics that a project exports alongside its own backend.
   Traces, spans and logs are dropped in memory. Only request volume, status codes and latency
   are kept, as aggregates.
3. **One shared view**: each project sees its own data only. Designated SCF operators compare
   the same standardized metrics across all enrolled projects.

Calistar is at the **proposal stage**. The landing page and a draft of the documentation are
online. The service itself is not built yet, and enrollment is not open.

## Repositories

| Repo                                                  | What it is                                                                                                                                  |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| [**calistar**](https://github.com/Calistar-io/calistar) | The monorepo. Today: the landing page and the documentation site. Planned: the console, the gateway, the tracker and the infrastructure as code. |

All code is to be released under an OSI-approved open-source license. The license is not chosen yet.

## Learn more

- [Architecture](https://calistar.io/docs/architecture/): the components and how data travels through them
- [For builders](https://calistar.io/docs/tenants/): what a project gets, what it adds to its site and its API
- [For operators](https://calistar.io/docs/operators/): the global view, running the service, handover
- [Security](https://calistar.io/docs/security/): tenant isolation, protection against inflated numbers, supply chain
- [Privacy](https://calistar.io/docs/privacy/): what is stored and never stored, draft compliance position
