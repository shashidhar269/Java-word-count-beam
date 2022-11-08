https://beam.apache.org/get-started/quickstart-java/

mvn archetype:generate `
  -D archetypeGroupId=org.apache.beam `
  -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
  -D archetypeVersion=2.42.0 `
  -D groupId=org.example `
  -D artifactId=word-count-beam `
  -D version="0.1" `
  -D package=org.apache.beam.examples `
  -D interactiveMode=false
   
cd .\word-count-beam

dir .\src\main\java\org\apache\beam\examples

In the word-count-beam directory, create a file called sample.txt. Add some text to the file. For this example

mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
 -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner

ls counts*
   
more counts*

Output :

KING: 9
mortal: 1
tell: 1
should: 3
day: 1
behaved: 1
who: 2
enough: 2
wrong: 1
tune: 1
delay: 1
variable: 1
Love: 1
further: 1
sent: 1
confession: 1
translate: 1
likeness: 1
you: 29
o: 4
joy: 1
turbulent: 1
kind: 1
yourselves: 1
mind: 3
doors: 1
bestow: 2
days: 1
Like: 1
pangs: 1
You: 2
fool: 2
d: 9
under: 1
right: 1
little: 1
I: 32
she: 1
Take: 1
fly: 1
never: 1
How: 3
origin: 1