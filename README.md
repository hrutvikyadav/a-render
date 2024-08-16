# a-render

## Demo website for rendering asciinema recordings

### Purpose

Already using asciinema to record terminal sessions. Needed to share those with a co.
Tried converting to `gif` it is terrible (no controls)
Tried gif -> mp4 with `ffmpeg`, need to find supported codecs for windows first
Tried cast -> mp4, previous steps are recommended
*Finally* settled for embedding the asciinema player in our own website
> There are multiple options
> - just use standalone js bundle __( current choice )__
> - npm package

### Standalone bundle

```bash
wget -O asciinema-player.min.js https://github.com/asciinema/asciinema-player/releases/download/v3.6.3/asciinema-player.min.js
wget -O asciinema-player.css https://github.com/asciinema/asciinema-player/releases/download/v3.6.3/asciinema-player.css
```

## References
[asciinema documentation](https://docs.asciinema.org/manual/player/quick-start/#standalone-player-bundle)

### Bugwarrior installation
This is complementary to the cast file

#### Taskwarrior
- [taskwarrior docs](https://taskwarrior.org/docs/) for usage and all advanced configuration

#### Bugwarrior
- [install bugwarrior](https://bugwarrior.readthedocs.io/en/latest/getting.html)
- [general bugwarrior configuration](https://bugwarrior.readthedocs.io/en/latest/common_configuration.html)
- [cli usage](https://bugwarrior.readthedocs.io/en/latest/manpage.html#)

#### JIRA
- [generating and using jira api tokens](https://support.atlassian.com/atlassian-account/docs/manage-api-tokens-for-your-atlassian-account/#Use-an-API-token)
- [jira query language - JQL](https://support.atlassian.com/jira-service-management-cloud/docs/use-advanced-search-with-jira-query-language-jql/) for the **issues query** in `bugwarriorrc`
- [setup jira for bugwarrior](https://bugwarrior.readthedocs.io/en/latest/services/jira.html) as it is *not available by default*

#### Github
- [generating and using github tokens](https://github.com/settings/tokens)
- [setup personal github for bugwarrior](https://bugwarrior.readthedocs.io/en/latest/services/github.html) just for testing

##### TODO
change the [description template](https://bugwarrior.readthedocs.io/en/latest/common_configuration.html#field-templates) by refering to JIRA UDA so that the `task list` description shows only what we want to see
> Ex. just issue number and description

### Postgres
[Install postgresql and enable peer authentication](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-22-04)

### Docker
[Install from docker's apt repository](https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository)
> [!note] other installation methods are available in docs

Check this if you want to run docker as non-root user **or** to run the docker daemon as a non-root user(Rootless mode)
[Docker post-install](https://docs.docker.com/engine/install/linux-postinstall/)

### Devpod
[Devpod cli installation](https://devpod.sh/docs/getting-started/install#optional-install-devpod-cli)
[Quickstart Neovim](https://devpod.sh/docs/getting-started/quickstart-vim)
