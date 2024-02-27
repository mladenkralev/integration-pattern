# Pipes and Filter integration pattern
Summary
- Pluses 
  - Allows isolated components to process messages in parallel way
  - Increasing cohesion of modules
  - Increasing integrability
  - Increasing modifiability
- Negatives
  - Increasing costs
  - Increasing complexity - multiple pipes, multiples components

![Alt text here](images/PipesAndFilters.svg)
# Message router
Summary
- Pluses
    - Single point component responsible for decision making 
    - Increasing cohesion of modules
    - Increasing integrability
    - Increasing modifiability
- Negatives
    - Increasing costs
    - Increasing complexity - multiple pipes, multiples components

![Alt text here](images/MessageRouter.drawio.svg)
![Alt text here](images/MessageTranslator.drawio.svg)
![Alt text here](images/MessagEndpoint.drawio.svg)

# Publish and Subscribe
Summary
- Pluses
    - Allows broadcasting messages to different subscribers
    - Decouples publisher from subscriber
- Negatives
  - None

![Alt text here](images/PublishSubscribe.drawio.svg)


![Alt text here](images/PointToPoint.drawio.svg)




![Alt text here](images/InvalidMessage.drawio.svg)
![Alt text here](images/DeadLetter.drawio.svg)