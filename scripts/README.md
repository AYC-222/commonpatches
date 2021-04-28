# Updating the Android Mainline Patch Series

1. Checkout the current base commit of the series (see series file)

   $ git checkout v5.12

2. Create a symbolic link to the patches subdirectory of android-mainline

   $ ln -s <path to common-patches repo>/android-mainline/ patches

3. Import the series into git

   $ git quiltimport

4. Do any necessary additions or transformations

5. Update the series. Make sure you use the correct base commit (e.g. after a
   rebase)

   $ <path to common-patches repo>/scripts/update_series.sh v5.12

