## Andrew Ng's Machine Learning Course at Stanford (through Coursera) -- Fall 2016
- This repo contains all my assignments for this course.

- Using Octave (open source version of Matlab)
---------------

For Windows users:

1) In the exercise /lib folder, edit and save the file submitWithConfiguration.m, changing line 66 from this:


responseBody = urlread(submissionUrl, 'post', params);




to

[code, responseBody] = system(sprintf('echo jsonBody=%s | curl -k -X POST -d @- %s', body, submissionUrl));


2) Then restart Octave.

----------------
