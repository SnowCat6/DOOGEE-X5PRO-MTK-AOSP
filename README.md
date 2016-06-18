Prepare folder, you must download MTK source code from internet and unpack into this place.
Make folder for source code of AOSP MTK
> mkdir alps
> cd alps

initialize REPO with sources 
> repo init -u git@github.com:SnowCat6/DOOGEE-X5PRO-MTK-AOSP.git
> repo sync -j4

make AOSP android 5.x or 6.x - automatic detection settings
> . build/envsetup.sh
 for x32 AOSP
> lunch full_X5PROx32-user && make -j4
for x64 AOSP
> lunch full_X5PROx64-user && make -j4

Good like!
