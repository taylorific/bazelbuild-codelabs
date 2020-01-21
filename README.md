# bazelbuild-codelabs

```
# Install Bazel
sudo apt install curl
curl https://bazel.build/bazel-release.pub.gpg | sudo apt-key add -
echo "deb [arch=amd64] https://storage.googleapis.com/bazel-apt stable jdk1.8" | sudo tee /etc/apt/sources.list.d/bazel.list
sudo apt update && sudo apt install bazel
# Install buildifier
git clone https://github.com/bazelbuild/buildtools
cd buildtools
bazel build //buildifier
bazel-bin/buildifier/linux_amd64_stripped/buildifier
# Install buildozer
#
git config --global user.email "taylorific@lain.ca"
git config --global user.name "Mischa Taylor"
git clone -b 0.23.2
https://github.com/bazelbuild/codelabs.git
#
bazel query
bazel build
bazel test
bazel run
```
