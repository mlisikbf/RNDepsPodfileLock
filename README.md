## Instructions

clone the repository and run pod install - note changes in Podfile.lock:
```
git clone git@github.com:mlisikbf/RNDepsPodfileLock.git
cd RNDepsPodfileLock
npm i && (cd ios; pod install; cd -)
git diff
```

pull another clone into a different dir - note changes in Podfile.lock do not match the other clone:
```
git clone git@github.com:mlisikbf/RNDepsPodfileLock.git RNDepsPodfileLock2
cd RNDepsPodfileLock2
npm i && (cd ios; pod install; cd -)
git diff
```