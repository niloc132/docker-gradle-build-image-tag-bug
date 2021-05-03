Demonstration for a bug in https://github.com/bmuschko/gradle-docker-plugin/, where the
DockerBuildImage task incorrectly believes itself to be up to date in some cases - as
long as the image still exists, even if it isn't tagged correctly any longer, the plugin
will leave the task marked "UP-TO-DATE".
