# *Ahoy!* 👋

Welcome to my GitHub profile.
This is the best place to find all my stuff while I finish setting up
    [my personal website & blog].
Read on for more information and all of the links.

If you haven't already guessed, I'm a software developer.
I also sometimes do scientific research — mostly about bats 🦇 —
and I like to write and teach about programming and data science.
For the full story, take a sneak peak at my [about me] article.
My [resume] is also available.

## Weblog
You can actually find all my articles [here], on GitHub.
I'm slowly collecting development logs, tutorials, and other long-form articles
    about my various interests.
Eventually, there will be a nice place to read them all on my personal website.
But, my [weblog repository] will still be the canonical source.

## Projects
Right now I'm deep in the process of building my personal website to host my
    blog content.
The project has two main components:
- a generic blog/portfolio template, [`blank`](#blank);
- and the deployment pipeline which configures and deploys the template,
    [`folio`](#folio).

If you're curious about the end goal, you can check out the [design file].

### <a id="blank"></a>[`blank`]
As a personal philosophy, I believe anything can be repurposed.
While building out my personal website, I chose to abstract out anything
    specific to myself.
The result was a opinionated, minimalistic template for a personal blog
    and/or portfolio.

The application uses the meta-framework [SvelteKit], to build a
    server-side rendered web application.
Page generation is configured at runtime to provide real-time updates to
    content, themes, and other application settings.

I am developing the template features alongside my personal website.
The planned features include:
- [x] Themeable palettes, typography, layouts, and graphics;
- [ ] Multiple theme support;
- [ ] Git integration for content management;
- [ ] Markdown blog posts/articles rendering;
- [ ] Ad-hoc static HTML pages.

### <a id="folio"></a>[`folio`]
My personal website serves as an ideal example for the `blank` template.
And in turn the `folio` repository defines a deployment pipeline to configure
    and deploy the `blank` template,
complete with config files, content, and instructions for setting up a
    deployment environment.

The deployment pipeline relies heavily on the included BASH scripts to
    automate [Docker] container builds and run [Terraform] deployments.
It also includes:
- [x] Automated tests for all application, pipeline functionality, and
    environment state;
- [x] GitHub commit status integration;
- [x] Optional GitHub actions workflows for automated CI/CD;
- [x] Concurrent deployment environments;
- [x] Automated TLS certificate provisioning (via [Caddy]);
- [x] [Sentry] error monitoring integration;
- [x] [Grafana Loki] application log aggregation;
- [ ] Integrated CDN provisioning;
- [ ] Configurable hosting providers
(currently requires [DigitalOcean], [GCS], and [Cloudflare] accounts).

## Contact
Feel free to reach out:
- ✉️ carl@carledwardlyons.ca
- 💼 [LinkedIn]

[my personal website & blog]: https://carledwardlyons.ca
[about me]:
    https://github.com/systemcarl/weblog/blob/main/articles/about-me.md
[resume]: https://systemcarl.github.io/profile/resume.html
[here]: https://github.com/systemcarl/weblog/tree/main/articles
[weblog repository]: https://github.com/systemcarl/weblog
[`blank`]: https://github.com/systemcarl/blank
[`folio`]: https://github.com/systemcarl/folio
[design file]:
    https://www.figma.com/design/TJYtbshPU4K0CoXuYKqtwp/Portfolio?node-id=109-188&t=w7DTuyIlvDiZi8pi-1
[SvelteKit]: https://svelte.dev/docs/kit/introduction
[Docker]: https://www.docker.com/
[Caddy]: https://caddyserver.com/
[Terraform]: https://developer.hashicorp.com/terraform
[Sentry]: https://sentry.io/
[Grafana Loki]: https://grafana.com/oss/loki/
[DigitalOcean]: https://www.digitalocean.com/
[GCS]: https://cloud.google.com/storage
[Cloudflare]: https://www.cloudflare.com/
[LinkedIn]: https://www.linkedin.com/in/celyons
