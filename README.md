# BB_Philosophy
I've uploaded some sample documents of my communication and general opinions on test design, workflow and ci/cd processes

This is only a first draft but as I persue more leadership roles it becomes increasingly important to understand my broad hopes and aspirations for quality in software development

So as a quick sample of my thinking here's some of my ideas:

CI/CD is so important!! I am a Paladin of CI/CD 

While there are still Saas and other applications where CI/CD are less important because its easy to create dumb customers etc in the docker cluster or the cloud, I am strongly in the camp that CI/CD is the right way to get good test coverage and generally increase quality

Canary Deployments:
Canary deployments are impotant but picking your least favorite customer as a POC, won't work well if the Canary is the smallest and newest of the customers. Because the oldest of the customers is most likely the one with the most complexity and largest number of old upgrade legacy artifacts that people forget exist. 

Picking a good canary can be more difficult than shoping for a car, and depending on the code changes being deployed, the canary order should also reflect those differences.

Custom code/features/customer requirements:
Creating a massive matrix of feature flags and custom code is a powderkeg that undermines the effectiveness of automation.
There are practical limits where relying on feature flags will either duplciate effort and code, or introduce a failure for something that "wouldnt affect the custoemrs" 
