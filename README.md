# vaadin8-poc

1) Create Vaadin sample project

mvn archetype:generate \
   -DarchetypeGroupId=com.vaadin \
   -DarchetypeArtifactId=vaadin-archetype-liferay-portlet \
   -DarchetypeVersion=8.14.3 \
   -DgroupId=com.pany \
   -DartifactId=vaadin-test-portlet \
   -Dversion=0.1

2) Changes in pom.xml

vaadin.plugin.version 8.17.0
liferay.kernel.version 29.0.0

Comment: Vaadin version 8.17.0 supports Liferay 7.4 U1 (kernel 29.0.0) in vaadin-server library's bnd.bnd as per
https://github.com/vaadin/framework/blob/8.17.0/server/bnd.bnd

3) mvn package

4) install.sh for Liferay 7.4 deployment (blade should be installed)
