# Pipes and Filter integration pattern
![Alt text here](images/PipesAndFilters.svg)
Summary
- Pluses 
  - Allows isolated components to process messages in parallel way
  - Increasing cohesion of modules
  - Increasing integrability
  - Increasing modifiability
- Negatives
  - Increasing costs
  - Increasing complexity - multiple pipes, multiples components

# Message router
![Alt text here](images/MessageRouter.drawio.svg)
Summary
- Pluses
    - Single point component responsible for decision making 
    - Increasing cohesion of modules
    - Increasing integrability
    - Increasing modifiability
- Negatives
    - Increasing costs
    - Increasing complexity - multiple pipes, multiples components


# Message translator
![Alt text here](images/MessageTranslator.drawio.svg)
Summary
- Pluses
  - Decouples components
  - Increases **_interoperability_** (ability of different systems, devices, applications, or products to communicate and work together effectively, even if they were developed by different manufacturers)
  - Similar to adapter pattern in GOF


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

# Guaranteed delivery
![Alt text here](images/GuaranteedDelivery.drawio.svg)
Summary
- Pluses
  - Ensures that the message is delivered
  - Ensures that the message is delivered only once
  - Ensures that the message is delivered in order
- Negatives
  - None
  - **_Note:_** This is a broker concern

# Channel adapter
![Alt text here](images/ChannelAdapter.drawio.svg)
Summary
- Pluses
  - Decouples the system from the external system
  - Increases **_interoperability_** (ability of different systems, devices, applications, or products to communicate and work together effectively, even if they were developed by different manufacturers)
  - Similar to adapter pattern in GOF
- Negatives
  - None 

# Message bridge
![MessageBrdige.drawio.svg](images/MessageBrdige.drawio.svg)
Summary
- Pluses


# Document Message
![DocumentMessage.drawio.svg](images/DocumentMessage.drawio.svg)
- Pluses
    - Allows to send a document as a message
- Negatives
    - None

# Command Message
![CommandMessage.drawio.svg](images/CommandMessage.drawio.svg)
- Pluses
    - Allows to send a command as a message
- Negatives
  - None


# Event Message
![EventMessage.drawio.svg](images/EventMessage.drawio.svg)
- Pluses
    - Allows to send a event as a message
  - Negatives
    - None

# Request-Reply
![RequestReply.drawio.svg](images/ReturnAdress.drawio.svg)  
- Pluses
    - Allows to send a request and get a reply
  - Negatives
    - None

# Return Address
![ReturnAdress.drawio.svg](images/ReturnAdress.drawio.svg)
- Pluses
    - Allows to send a request and get a response
  - Negatives
    - None


