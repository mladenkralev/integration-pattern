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
# Message translator

Summary
- Pluses
  - Decouples components
  - Increases **_interoperability_** (ability of different systems, devices, applications, or products to communicate and work together effectively, even if they were developed by different manufacturers)
  - Similar to adapter pattern in GOF

![Alt text here](images/MessageTranslator.drawio.svg)

# Message endpoint
![Alt text here](images/MessagEndpoint.drawio.svg)
Summary
- Message broker handling channel logic
- Message endpoint handling eather sending or receiving logic
- Increasing separating of concerns, increasing cohesion, decreasing coupling

# Publish and Subscribe
![Alt text here](images/PublishSubscribe.drawio.svg)
Summary
- Pluses
  - Allows broadcasting messages to different subscribers
  - Decouples publisher from subscriber
- Negatives
  - None


# Point to point channel
![Alt text here](images/PointToPoint.drawio.svg)

Summary
- Pluses
  - Mimics RPC calls, but it does not wait for response. Can be combined with document, command or other message types
  - Ensures one and only one consumer
  - Async communication
- Negatives
  - None


# Invalid message channel
![Alt text here](images/InvalidMessage.drawio.svg)
Summary
- Pluses
  - Way to indicate that the messages are not okay for processing in a graceful way
  - Separates valid and invalid messages
  - **Application concern.** Consumes the message and then sees if the message is valid and invalid
- Negatives
  - None

# Dead letter channel
![Alt text here](images/DeadLetter.drawio.svg)
Summary
- Pluses
  - Way to indicate that the messages are not okay for processing in a graceful way
  - Separates valid and invalid messages
  - **Message broker concenrn** If broker cannot proceed with consuming the message it must indicate in a way there is a error
- Negatives
  - None