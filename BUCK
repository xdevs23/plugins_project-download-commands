include_defs('//bucklets/gerrit_plugin.bucklet')

gerrit_plugin(
  name = 'project-download-commands',
  srcs = glob(['src/main/java/**/*.java']),
  resources = glob(['src/main/resources/**/*']),
  manifest_entries = [
    'Gerrit-PluginName: project-download-commands',
    'Gerrit-Module: com.googlesource.gerrit.plugins.download.command.project.Module',
    'Implementation-Title: Project download command plugin',
    'Implementation-URL: https://gerrit-review.googlesource.com/#/admin/projects/plugins/project-download-commands',
  ]
)
# this is required for bucklets/tools/eclipse/project.py to work
java_library(
  name = 'classpath',
  deps = [':project-download-commands__plugin'],
)

