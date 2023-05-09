# leshan-core的关键类

## 请求相关
* org.eclipse.leshan.core.request.LwM2mRequest
* |-org.eclipse.leshan.core.request.DownlinkRequest
* |-org.eclipse.leshan.core.request.UplinkRequest

## 响应相关
* org.eclipse.leshan.core.response.LwM2mResponse
* org.eclipse.leshan.core.response.ErrorCallback
* org.eclipse.leshan.core.response.ResponseCallback

## 关键概念落地类
* org.eclipse.leshan.core.request.Identity
* org.eclipse.leshan.core.attributes.Attribute
* org.eclipse.leshan.core.model.LwM2mModel
* org.eclipse.leshan.core.model.URN
* org.eclipse.leshan.core.node.LwM2mNode
* org.eclipse.leshan.core.node.LwM2mResource
* org.eclipse.leshan.core.observation.Observation

## Core
* org.eclipse.leshan.server.californium.request.CoapRequestBuilder
* org.eclipse.leshan.core.tlv.TlvDecoder
* org.eclipse.leshan.core.tlv.TlvEncoder

## 协议相关
* org.eclipse.leshan.core.request.ContentFormat
* org.eclipse.leshan.core.ResponseCode
* org.eclipse.leshan.core.SecurityMode

## 协议负载编解码
* org.eclipse.leshan.core.node.codec.LwM2mNodeDecoder
* org.eclipse.leshan.core.node.codec.LwM2mNodeEncoder

# leshan-server-core的关键类

## 框架类
* org.eclipse.leshan.server.security.Authorizer
* org.eclipse.leshan.server.security.DefaultAuthorizer
* org.eclipse.leshan.server.security.SecurityStore
* org.eclipse.leshan.server.registration.RegistrationService
* org.eclipse.leshan.server.registration.RegistrationStore
* org.eclipse.leshan.server.registration.RegistrationListener
* org.eclipse.leshan.server.registration.RegistrationIdProvider
* org.eclipse.leshan.server.registration.PresenceService
* org.eclipse.leshan.server.registration.PresenceListener
* org.eclipse.leshan.server.registration.ObservationListener
* org.eclipse.leshan.server.registration.ObservationService

## 关键概念落地类
* org.eclipse.leshan.server.security.SecurityInfo
* org.eclipse.leshan.server.registration.Registration
* org.eclipse.leshan.server.registration.RegistrationUpdate
* org.eclipse.leshan.server.registration.Deregistration
* org.eclipse.leshan.server.model.LwM2mModelProvider

# leshan-server-cf的关键类

## 框架相关类
* org.eclipse.leshan.server.californium.LeshanServer
* org.eclipse.leshan.server.californium.LeshanServerBuilder
* org.eclipse.leshan.server.californium.RootResource
* org.eclipse.leshan.server.californium.request.CoapRequestBuilder
* org.eclipse.leshan.server.californium.request.CoapRequestSender

# leshan-client-core的关键类

## 框架相关类
* org.eclipse.leshan.client.LwM2mClient
* org.eclipse.leshan.client.EndpointsManager
  
* org.eclipse.leshan.client.request.LwM2mRequestSender

## 关键概念落地类
* org.eclipse.leshan.client.servers.ServerIdentity
* org.eclipse.leshan.client.resource.LwM2mObjectEnabler
* org.eclipse.leshan.client.resource.LwM2mObjectEnabler2
* org.eclipse.leshan.client.resource.LwM2mInstanceEnabler
* 
* 





