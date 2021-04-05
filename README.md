# TiEtwAgent

This project was build to research, build and test different memory injection detection usecases utilizing Microsoft-Windows-Threat-Intelligence event tracing provider, as a more modern and stable alternative to Userland-hooking, with the benefit of Kernel-mode visibility. The project uses the [microsoft/krabsetw](https://github.com/microsoft/krabsetw) library for ETS setup and consumption.

An accompanying blog post can be found here: https://blog.redbluepurple.io/windows-security-research/kernel-tracing-injection-detection

![gif](https://i.imgur.com/M9QXk1z.gif)

### Implemented detection usecases 
- [x] ALLOCVM_REMOTE_META_GENERIC - Simple detection based on allocation type, protection mask and size threashold of a newly allocated remote memory page
- [ ] ALLOCVM_REMOTE_SIGNATURES - Simple Yara-based detection
- [ ] APC detections
- [ ] Process hollowing detections
- [ ] ...

### TODO
- [x] PPL Service, event parsing 
- [x] First detection  
- [ ] Ingegrate Yara and scanning
- [ ] Rewrite with OOP 
- [ ] Detection lifecycle 
- [ ] Risk based detection lifecycle 

### Setup instructions