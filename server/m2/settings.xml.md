Maven settings configuration file
### Local Repository (`localRepository`)
- Specifies the path to the local Maven repository where artifacts are stored
- Currently set to `${env.REPO_ROOT}/server/.m2/repository` using the `REPO_ROOT` environment variable to determine the location
### Interactive Mode (`interactiveMode`):
- Determines whether Maven will prompt the user for input during builds
- It is set to `true` by default
### Offline Mode (`offline`)
- Determines whether Maven should attempt to connect to the network when building
### Plugin Groups (`pluginGroups`)
- Specifies additional groups to search for plugins.
### Proxies (`proxies`)
- Configures network proxies for Maven to use when connecting to the internet.
### Servers (`servers`)
- Defines authentication information for connecting to remote servers.
- Includes placeholders for authentication credentials for servers.
### Mirrors (`mirrors`)
- Directs Maven to different download locations if the main repository is slow or unreliable in providing artifacts
### Profiles (`profiles`)
- Defines build profiles that can be activated under certain conditions
### Active Profiles (`activeProfiles`)
- Specifies profiles that should be active by default for all Maven builds