# Readme

This is a demo exerpt from a low-code BPMS platform help.

The excerpt is imported from MkDocs.

GitBook view link: [https://arterm-sedov.gitbook.io/help-sample/](https://arterm-sedov.gitbook.io/help-sample/)

GitHub repository: [https://github.com/arterm-sedov/gitbook-cmw-excerpt/](https://github.com/arterm-sedov/gitbook-cmw-excerpt/)

## Task&#x20;

From the ground up, create docs-as-code context- and locale-aware help for a low-code business application platform. Integrate help authoring with knowledgebase, version control and CI/CD workflows.

## Input

I was provided with the testbed and real-world business apps powered by the CMW Business Application Platform, and platform source code.

## Process

1. I've explored the platform codebase to determine which documentation framework would be suitable and maintainable in the long term for our product.\

2. After consulting with the developers, system analysts, content creators, and product owner, I've suggested suitable single source docs-as-code frameworks that would fit all or most requirements.
3. We've opted for MkDocs paired with the well-supported Material for MkDocs theme for its simplicity, wide adoption, and expandability.
4. Among the requirements were context and awareness of the help system: when the user taps the Help button, they should see an article relevant to the platform page they're viewing and in the current platform language. To implement this functionality, I coded a JavaScript help path resolver that uses the platform's module and localization services to determine the path to the help page in the required language.
5. When the help framework was ready for authoring, I developed Python, JavaScript, and shell scripts to integrate the MkDocs build steps into our product build pipeline for Windows and Linux.
6. As the product has different branding for different markets, the help content is brand-agnostic and parametrized (including brand names, CSS, fonts, icons, and colors): all branded items are configured in YML files.
7. The help system also inherits the CSS styles of the host platform, so it looks in line with the themes our customers develop for their apps powered by the CMW platform.&#x20;
8. We use VS Code and Git to author, review, and approve the help content.
9. I've created scripts to parse and import articles from the MkDocs help to the PHPKB-powered knowledge base.

## Result

60k+ words and 1k+ screenshots MkDocs help system, a help context resolver and a cross-platform build agent that support multiple languages and adhere to the host platform context and theme.

<figure><img src="https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/04bf24154918333.634afd8559911.png" alt=""><figcaption><p>Python help build script</p></figcaption></figure>

<figure><img src="https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/35f712154918333.634afd8558ccf.png" alt=""><figcaption><p>Help context and language JavaScript resolver</p></figcaption></figure>

<figure><img src="https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/4172d4154918333.63a34f08cc151.png" alt=""><figcaption><p>Help article markdown source</p></figcaption></figure>
