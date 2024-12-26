# Docker Komutları - Soru ve Cevapları

1. Docker'da çalışan tüm containerları listelemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker ps -a
</details>

2. Bir Docker imajını yerel registry'den silmek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker rmi <image_name>
</details>

3. Docker container'ı interaktif modda başlatmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run -it <image_name>
</details>

4. Docker üzerinde çalışan bir container'ı durdurmak için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker stop <container_id/name>
</details>

5. Docker container'ın sistem kaynak kullanımını görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker stats
</details>

6. Bir Docker imajını DockerHub'dan çekmek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker pull <image_name>
</details>

7. Docker container'ı arkaplanda (detached mode) çalıştırmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run -d <image_name>
</details>

8. Docker container'ın loglarını görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker logs <container_id/name>
</details>

9. Çalışan bir Docker container'ına bağlanmak için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker attach <container_id/name>
</details>

10. Docker container'ı özel bir port ile çalıştırmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run -p host_port:container_port <image_name>
</details>

11. Docker container'ın içindeki bir dosyayı host sisteme kopyalamak için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker cp <container_id>:/path/to/file /host/path
</details>

12. Docker imajlarını yerel registry'de listelemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker images
</details>

13. Docker container'ı belirli bir isimle başlatmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --name <container_name> <image_name>
</details>

14. Docker container'ın çalışma durumunu kontrol etmek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker inspect <container_id/name>
</details>

15. Docker container'ı otomatik olarak yeniden başlatmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --restart always <image_name>
</details>

16. Docker container'ın kullandığı ağ ayarlarını görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker network inspect <network_name>
</details>

17. Yeni bir Docker network oluşturmak için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker network create <network_name>
</details>

18. Docker container'a environment variable eklemek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run -e KEY=VALUE <image_name>
</details>

19. Docker volume oluşturmak için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker volume create <volume_name>
</details>

20. Docker container'a volume bağlamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run -v <volume_name>:/container/path <image_name>
</details>

21. Docker imajını build etmek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker build -t <image_name> .
</details>

22. Docker container'ın çalışma dizinini değiştirmek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run -w /path/to/workdir <image_name>
</details>

23. Docker container'da komut çalıştırmak için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker exec -it <container_id/name> <command>
</details>

24. Docker container'ın kullandığı tüm portları görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker port <container_id/name>
</details>

25. Docker container'ı silerek durdurmak için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker rm -f <container_id/name>
</details>

26. Docker system bilgilerini görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker system info
</details>

27. Docker disk kullanımını görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker system df
</details>

28. Docker container'ı belirli bir kullanıcı olarak çalıştırmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run -u <username/uid> <image_name>
</details>

29. Docker imajını tag'lemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker tag <source_image> <target_image>
</details>

30. Docker container'ın history bilgisini görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker history <image_name>
</details>

31. Docker container'a host makinesinin DNS ayarlarını kullanmasını sağlamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --dns <dns_server> <image_name>
</details>

32. Docker container'ın memory limitini belirlemek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --memory <limit> <image_name>
</details>

33. Docker container'ın CPU kullanımını sınırlamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --cpus <value> <image_name>
</details>

34. Docker container'a host makinesinin hostname'ini vermek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --hostname <hostname> <image_name>
</details>

35. Docker container'ın çalışma zamanını görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker ps -a --format "{{.Names}} {{.RunningFor}}"
</details>

36. Docker imajını DockerHub'a göndermek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker push <image_name>
</details>

37. Docker container'ı read-only filesystem ile çalıştırmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --read-only <image_name>
</details>

38. Docker container'ın process ID'sini görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker inspect --format '{{.State.Pid}}' <container_id/name>
</details>

39. Docker container'a host makinesinin timezone'unu vermek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run -e TZ=<timezone> <image_name>
</details>

40. Docker container'ın ağ sürücüsünü değiştirmek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --network <network_driver> <image_name>
</details>

41. Docker container'a özel DNS search domain eklemek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --dns-search <domain> <image_name>
</details>

42. Docker container'ın restart politikasını görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker inspect --format '{{.HostConfig.RestartPolicy}}' <container_id/name>
</details>

43. Docker container'a host makinesinin /etc/hosts dosyasını eklemek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --add-host <hostname:ip> <image_name>
</details>

44. Docker container'ın environment variables'larını görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker inspect --format '{{.Config.Env}}' <container_id/name>
</details>

45. Docker container'ı privileged modda çalıştırmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --privileged <image_name>
</details>

46. Docker container'a özel ulimit değerleri atamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --ulimit <type>=<soft_limit>:<hard_limit> <image_name>
</details>

47. Docker container'ın çalıştığı host makinesini görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker inspect --format '{{.Node.Name}}' <container_id/name>
</details>

48. Docker container'a device bağlamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --device <host_device>:<container_device> <image_name>
</details>

49. Docker container'ın IP adresini görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker inspect --format '{{.NetworkSettings.IPAddress}}' <container_id/name>
</details>

50. Docker container'ı belirli bir MAC adresi ile başlatmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --mac-address <mac_address> <image_name>
</details>

51. Docker container'a özel security-opt parametreleri eklemek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --security-opt <key>=<value> <image_name>
</details>

52. Docker container'ın çalıştığı platform bilgisini görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker inspect --format '{{.Platform}}' <container_id/name>
</details>

53. Docker container'a tmpfs mount eklemek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --tmpfs <mount_path> <image_name>
</details>

54. Docker container'ın kullandığı sysctl parametrelerini görüntülemek için hangi komut kullanılır?
<details>
<summary>Cevap</summary>
docker inspect --format '{{.HostConfig.Sysctls}}' <container_id/name>
</details>

55. Docker container'a özel grup ID'si atamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --group-add <group_id> <image_name>
</details>

56. Docker container'ın pid namespace'ini host ile paylaşmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --pid=host <image_name>
</details>

57. Docker container'ın IPC namespace'ini host ile paylaşmak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --ipc=host <image_name>
</details>

58. Docker container'a özel shm-size değeri atamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --shm-size <value> <image_name>
</details>

59. Docker container'ın oom-kill-disable özelliğini aktifleştirmek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --oom-kill-disable <image_name>
</details>

60. Docker container'a özel oom-score-adj değeri atamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --oom-score-adj <value> <image_name>
</details>

61. Docker container'ın pid limitini belirlemek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --pids-limit <value> <image_name>
</details>

62. Docker container'a cgroup-parent atamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --cgroup-parent <path> <image_name>
</details>

63. Docker container'ın blkio-weight değerini belirlemek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --blkio-weight <value> <image_name>
</details>

64. Docker container'a özel kernel memory limiti atamak için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --kernel-memory <value> <image_name>
</details>

65. Docker container'ın memory reservation değerini belirlemek için hangi parametre kullanılır?
<details>
<summary>Cevap</summary>
docker run --memory-reservation <value

66. Docker container'a swap memory limiti atamak için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --memory-swap <value> <image_name>
</details>

67. Docker container'ın CPU shares değerini belirlemek için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --cpu-shares <value> <image_name>
</details>

68. Docker container'a CPU period limiti atamak için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --cpu-period <value> <image_name>
</details>

69. Docker container'ın CPU quota değerini belirlemek için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --cpu-quota <value> <image_name>
</details>

70. Docker container'a özel cpuset-cpus değeri atamak için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --cpuset-cpus <value> <image_name>
</details>

71. Docker container'a özel cpuset-mems değeri atamak için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --cpuset-mems <value> <image_name>
</details>

72. Docker container'ın device write bps limitini belirlemek için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --device-write-bps <value> <image_name>
</details>

73. Docker container'ın device read bps limitini belirlemek için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --device-read-bps <value> <image_name>
</details>

74. Docker container'ın device write IOPS limitini belirlemek için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --device-write-iops <value> <image_name>
</details>

75. Docker container'ın device read IOPS limitini belirlemek için hangi parametre kullanılır?

<details>
<summary>Cevap</summary>
docker run --device-read-iops <value> <image_name>
</details>
