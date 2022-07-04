# Accelerator Log

## Options
```json
{
  "deploymentType" : "manifest",
  "message" : "World",
  "projectName" : "SCM-Tanzu-Test"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ Debug .github/workflows/code-scan.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug grype.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**]
┃ ┃ ┃ ┃ ┃ Debug .github/workflows/code-scan.yml matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug grype.yaml matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┗ ┗ Debug tap/workload.yaml matched [pom.xml, README.md, grype.yaml, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ Debug .github/workflows/code-scan.yml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug grype.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [hello-world->SCM-Tanzu-Test]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'none') evaluated to false
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'manifest') evaluated to true
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'manifest') evaluated to true
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [cloudfoundry/manifest.yml]
┃ ┃ ┃ ┃ ┃ Debug .github/workflows/code-scan.yml didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml matched [cloudfoundry/manifest.yml] -> included
┃ ┃ ┃ ┃ ┃ Debug grype.yaml didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-world->SCM-Tanzu-Test, World->World]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┗ ┗ ┗ Debug Path 'cloudfoundry/manifest.yml' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.yml, folder=cloudfoundry/, filename=manifest.yml, g0=cloudfoundry/manifest.yml, g1=cloudfoundry/, g2=manifest.yml, g3=manifest.yml, g4=.yml} and was rewritten to 'config/manifest.yml'
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to false
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to false
┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┏ README (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(Append))
┃ ┃ ┃ ┃ README.merge (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┏ README.merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .github/workflows/code-scan.yml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug grype.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [hello-world->SCM-Tanzu-Test]
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'manifest') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'manifest') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [cloudfoundry/DEPLOYING.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .github/workflows/code-scan.yml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md matched [cloudfoundry/DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug grype.yaml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-world->SCM-Tanzu-Test]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ Debug Path 'cloudfoundry/DEPLOYING.md' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.md, folder=cloudfoundry/, filename=DEPLOYING.md, g0=cloudfoundry/DEPLOYING.md, g1=cloudfoundry/, g2=DEPLOYING.md, g3=DEPLOYING.md, g4=.md} and was rewritten to 'README.md'
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to false
┃ ┃ ┃ ┃ ┗ ┗ null ()
┃ ┃ ┃ ┃ ┏ README.merge.transformations[1] (UniquePath)
┃ ┃ ┗ ┗ ┗ Debug Multiple representations for path 'README.md', will concatenate them together
┃ ┗ ╺ engine.transformations[0].merge.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
