## Setting up and testing jekyll locally (Debian/Ubuntu).

1. Install ruby and ruby-dev

```
$ sudo apt -y install ruby ruby-dev
```

2. Set gem paths:

```
$ echo 'export GEM_HOME=$HOME/gems' >> ~/.bashrc
$ echo 'export PATH=$HOME/gems/bin:$PATH' >> ~/.bashrc
$ source ~/.bashrc
```

Note: On MacOS, you can install ruby and jekyll following the documentation:
https://jekyllrb.com/docs/installation/macos/
Then go to step 3.

3. Install bundler jekyll and rails

```
$ gem install bundler jekyll rails
```

4. Go to the directory of the webpage and initialize.

```
$ cd [path to srg-web]
$ bundle init
$ bundle add jekyll
$ bundle install
```

5. Note that the baseurl in the \_config.yml file for deployment and local testing should be configured differently: "/" for deployment and "" for local testing. The yml file is configured with baseurl "/".

6. To test the webpage locally use the command below. Note that the baseurl
   in the \_config.yml file is overridden using --baseurl "".

```
$ bundle exec jekyll serve --config _config.yml --baseurl ""
...
...
Server address: http://127.0.0.1:4000
...
```

7. On your local browser use the address from the output to access the page.

```
http://127.0.0.1:4000/
```

## Making changes to the group members

* The group member information is in the \_data directory as tsv (tab separated
  values) files.
* The first row of each file shows the attribute names of the members in the
  file.
* Add/remove/modify the information about group members following the existing
  tsv format.  
* The profile photos should be stored in images/faculty and images/students
  directories. Image file names in these directories should be referenced in the
  tsv files in the \_data directory to link the photo to the profile.
* Thumbnail photos from the people page of the Khoury College website are
  usually used as is. Their sizes are usually 287 x 161 px. If photos from 
  elsewhere should be used, the photo should be resized to have width of 287 px
  (height doesn't have to match 161). This is mainly to reduce the size of the
  image.

## Adding entries for internal paper reading group meetings

* The relevant information is in the \_data/readinggroups.tsv file.
* Add the new information following the existing format in the file. 

## Adding entries for seminars with external speaker

* The seminar information should be added as a file in the \_seminars directory.
* The easiest way is to copy an existing file in this directory and modifying
  the file name and the file contents.
    * The file name should be "**YYYY-MM-DD-\[Speaker's name\].md**" where
      YYYY-MM-DD corresponds to the seminar date. 
    * The file contains a header (or Jekyll front matter) with multiple fields,
      abstract, and bio. Modify the fields and contents of the abstract and the
      bio. The "online" field should be filled with either YES or NO.

## Adding entries for events 

* The relevant information is in the \_data/events.tsv file.
* Add the new information following the existing format in the file. 

## Adding entries to photos page 

* The relevant information is in the \_data/photos.tsv file.
* The photos should be uploaded to images/group\_photos directory. The photo
  width should be 1024 px.
* The file name of the photo should be added to the tsv file above.  

## Improvement ideas for the webpage

* Multi-page support: the seminars and photos pages can grow large as time goes 
  by. Adding multi-page navigation for them will become necessary.
* Image gallery: photos page can be made to follow a widely-used online image 
  gallery format which shows thumbnails and showing larger images when clicked.
  Currently, only one photo is uploaded per event due to lack of this feature.  
