

all:
	@echo make bld
	@echo make cln

ts:
	gradle generateTypeSystem

bld:
	gradle build

ecl:
	gradle eclipse
	sed -i.bak '/"generated-src\/jcasgen\/main"/d' .classpath

cln:
	rm -rf *~
	gradle clean
	gradle cleanEclipse
	rm -rf bin

cln-all: cln
	rm -rf .settings
	rm -rf .gradle

run1:
	gradle run1

run2:
	gradle run2

run3:
	gradle run3

