Demonstrate how to add large binary files in git using lfs:

# TESTED SUCCESSFULLY ON MAC

Git LFS is useful to handle large binary files efficiently.


## 1. Install Git LFS:*

pip install git-lfs

After installing, initialize Git LFS in your repository:

git lfs install

## 2. Create a Branch:**

git checkout -b lfs
git lfs track "*.bin"

This command creates a .gitattributes file in your current directory which provides info on Git LFS tracking files i.e. .bin files in this case.

## 3. Add, Commit, and Push to repo:

git add .gitattributes
git add *.bin
git commit -m "adding large binary file using git-lfs"
git push origin lfs

## 4. If incase we have not enabled git-lfs:

abhutoria@abhutor-ltmbqz4 git_assignment_HeroVired % git push origin test1            
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 14 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 224.66 MiB | 2.18 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: error: Trace: 14038d667cd0995fa603b2ffa94768b8eb0d45dc72b93a0f2c662342d5f1703f
remote: error: See https://gh.io/lfs for more information.
remote: error: File bfile.bin is 227.71 MB; this exceeds GitHub's file size limit of 100.00 MB
remote: error: GH001: Large files detected. You may want to try Git Large File Storage - https://git-lfs.github.com.
To github.com:akshaybhu/git_assignment_HeroVired.git
 ! [remote rejected] test1 -> test1 (pre-receive hook declined)
error: failed to push some refs to 'github.com:akshaybhu/git_assignment_HeroVired.git'
