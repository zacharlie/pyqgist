# PyGgist

A script template generator and content discovery framework for scripts which use the QGIS "PyQgis" API.

## [Go to the PyQgist App](https://zacharlie.github.io/pyqgist/)

## [Go to the Geogist App](https://zacharlie.github.io/geogist/)

## Guidelines for the design, storage and sharing of PyQgis Scripts

Scripts go by many names: snippets, gists or even clips. They come in many shapes (designs) and sizes (length) and perform any number of actions.

As not all scripts are created equal, they shouldn't be treated as such. The following list provides a guideline for how to create, store or search for content depending on it's design and purpose.

- [PyQgis Developer cookbook](https://docs.qgis.org/latest/en/docs/pyqgis_developer_cookbook): Various scripts, functions, templates and boilerplate code for performing common tasks used across various domains and adhering to the best practices as identified by QGIS.org and the core QGIS community.
- Curated content: As the content, quality, design and function of scripts may vary, individual developers may prefer to keep their own "curated collections" of scripts which perform a specific subset of actions, fill some industry specific purpose or adhere to a particular standard. As these requirements are typically rather subjective, they are handled by each developer independantly, but a centralised list for discovering these repositories is available from [awesome-pyqgis](https://github.com/zacharlie/awesome-pyqgis).
- [PyQgist](https://github.com/zacharlie/pyqgist): The bizarre, where users can share and discover code snippets by using [GitHub Gists](https://gist.github.com/) as a backend. The app simply provides some default tags and templates that conform to a standardised structure in oreder to help with consistency, as well as providing a simple search function which will prepopulate the GitHub search functionality and assist with code discovery.
- [GeoGist](https://github.com/zacharlie/geogist): PyQgist is intended sctrictly for snippets that use the QGIS Python (PyQgis) API, however users who wish to share and discover snippets for other spatial operations, such as PostGIS procedures, ArcPy scripts, or even shell scripts that are useful in a spatial data management context, can use the GeoGist application instead.

## Rationale

PyQgist is a community project, which attempts to provide a unified platform for the sharing and discovery of PyQGIS scripts and code snippets.

After [community discussion](http://osgeo-org.1560.x6.nabble.com/Shared-common-library-for-PyQGIS-scripts-td5448095.html#a5448117) initiated an attempt at reconciling the available methods of snippet sharing, a number of platforms and methods were evaluated with the intention of finding a single paltform which held all the following attributes:

- Frictionless: Users new and old should not have to deal with any learning curve and everything should be simple and copy-paste ready.
- Standardised: the styling, spelling and specifications should all be standardised to ensure that content is consistent and can be discovered easily.
- Resilient: A robust platform like GitHub should serve as the backend, rather than an independant platform that could disappear at any point.
- Open: In line with FOSS ideals, the platform should be open, and decentralised where possible.
- Low Infrastructure requirements: No infrastructure has been provisioned, so hosting on public infrastructure is required.

Although many snippet sharing platforms were evaluated, none of them managed to have a code tagging method which allowed multiple users to discover content by using the same shared tags.

After much deliberation, GitHub gists were identified as the best platform for sharing short code snippets that are potentially useful to a wide audience.

The application itself is a simple code template and search URL generator which utilises a series of preconfigured tags.

Once the GitHub Gists API supports tags or offers a GraphQL endpoint, this application may become redundant.

## Contributing

Don't make single line contributions like adding a single tag or inspirational message. Create an issue and discuss whether a tag(s) is worth including with others. If a number of new tags are to be included create a PR which consolidates multiple inputs and closes multiple issues, but you can expect single line changes to be ignored unless they are particularly useful.

You can also motivate for tags to be removed with a GitHub issue. This project is designed to be a community tool and not a marketing platform for any specific agency. The merit of a tag will be evaluated on it's utility.
