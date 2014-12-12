1) open the .target in eclipse 44.
2) export it to some TargetPlatformE44/
3) eclipse export fails to update the content.xml and artifact so we need to regenerate the p2 repository with the following command 
        Applications/java/eclipse/4.2/eclipse/eclipse -application org.eclipse.equinox.p2.publisher.FeaturesAndBundlesPublisher -metadataRepository file:/Applications/java/talend/TargetPlatformE44/p2site/ -artifactRepository file:/Applications/java/talend/TargetPlatformE44/p2site/ -source /Applications/java/talend/TargetPlatformE44 -config ANY -publishArtifacts 