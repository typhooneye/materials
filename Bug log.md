1. zipfile.BadZipFIle: File is not a zip file

  solution from [Chaithanya Kumar](https://stackoverflow.com/a/41916324)
  try: pip install --no-cache-dir <package_name>, it will work
  when you try to pip install , first pip will check the pip cache for the package. if the package is found and fresh, pip will grap the .whl file for the package and try to install. this results in badzipfile as a .zip file is excepted.
  try pip install in verbose mode pip install <some_package> -vvvv. you can see that it will first try to install from cache
