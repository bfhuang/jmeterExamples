The easiest way to install it is using Homebrew:
brew install jmeter
Or if you need plugins also:
brew install jmeter --with-plugins
And to open it, use the following command (since it doesn't appear in your Applications):
open /usr/local/bin/jmeter



view result tree listener, 是in memory的， 很消耗内存， 在做performance测试的时候最好不要用这个listener
Blaze meter to record the ui test


run jmeter from command line:
1.save the test plan first
2.jmeter -n -t testPlanFileLocation -l resultFileLocation（jmeter -n -t /Users/bfhuang/Downloads/jmeter/RunJmeterFromCommandLineTest.jmx -l  /Users/bfhuang/Downloads/jmeter/rumJmeterFromCmmandLineResult.csv）
-n  ->  non gui
-t -> the script location
-l the result location

generate html reports from test
 sh jmeter -n -t /Users/bfhuang/Downloads/jmeter/RunJmeterFromCommandLineTest1.jmx -l  /Users/bfhuang/Downloads/jmeter/rumJmeterFromCmmandLineResult2.csv  -e -o /Users/bfhuang/Downloads/jmeter/htmlReports  


generate html from cvs file
sh jmeter -g  /Users/bfhuang/Downloads/jmeter/rumJmeterFromCmmandLineResult3.csv  -o /Users/bfhuang/Downloads/jmeter/htmlReports33


https://www.youtube.com/watch?v=EUgLRmlkTGQ
