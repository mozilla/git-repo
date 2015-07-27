
The modification herein allows use of git ssh

= Manifest =

mkdir projdir && cd projdir
curl https://raw.githubusercontent.com/mozilla/git-repo/master/repo > ./repo
chmod u+x ./repo
./repo repo init -u git@github.com:githubuser/manifests.git
./repo sync

= Manifest =

<?xml version="1.0" ?>
<manifest>
  <remote fetch="git@github.com:mozilla/" name="mozilla"/>

  <project name="privaterepo" path="localpath/privaterepo" remote="mozilla" revision="master"/>
</manifest>