# ebextensions
Customizing and Configuring AWS Elastic Beanstalk (EBS) Environments

## How to Use
* Create .ebextensions directory under your project root.
* Copy the `*.config` files into the directory.
* Deploy project to EBS. 

## sidekiq
* Tested to be working on following configurations:-
  1. 64bit Amazon Linux 2015.03 v2.0.1 running Ruby 2.1 (Passenger Standalone).
  2. 64bit Amazon Linux 2015.03 v2.0.0 running Ruby 2.1 (Passenger Standalone).
  3. 64bit Amazon Linux 2015.03 v1.4.6 running Ruby 2.1 (Passenger Standalone).
  4. 64bit Amazon Linux 2015.03 v1.4.3 running Ruby 2.1 (Passenger Standalone).
  5. 64bit Amazon Linux 2015.03 v1.4.1 running Ruby 2.1 (Passenger Standalone).
  6. 64bit Amazon Linux 2015.03 v1.3.1 running Ruby 2.1 (Passenger Standalone).
  7. 64bit Amazon Linux 2015.03 v1.3.0 running Ruby 2.1 (Passenger Standalone).
  8. 64bit Amazon Linux 2014.09 v1.2.0 running Ruby 2.1 (Passenger Standalone).
* Need to set `RAILS_ENV` environment variable which is used in `0003_sidekiq.config`.
* [Source](https://gist.github.com/gcarrion-gfrmedia/11396682).

## Notes
* `option_settings` key [[1]](http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/ebextensions-optionsettings.html)
* Refer from the list of keys at [[2]](http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/customize-containers-ec2.html)
  * `packages` key [[3]](http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/customize-containers-ec2.html#linux-packages)
  * `container_commands` key [[4]](http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/customize-containers-ec2.html#linux-container-commands)
  * `files` key [[5]](http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/customize-containers-ec2.html#linux-files)
  * `commands` key [[6]](http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/customize-containers-ec2.html#linux-commands)
