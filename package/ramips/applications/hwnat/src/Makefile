EXEC = hwnat acl ac mtr

HWNAT_OBJS = hw_nat.o hwnat_api.o util.o
AC_OBJS = ac.o ac_api.o util.o
ACL_OBJS = acl.o acl_api.o util.o
MTR_OBJS = mtr.o mtr_api.o util.o

all: $(EXEC)

hwnat: $(HWNAT_OBJS) $(CONF_H)
	$(CC) $(LDFLAGS) -o $@ $(HWNAT_OBJS) 

acl: $(ACL_OBJS)
	$(CC) $(LDFLAGS) -o $@ $(ACL_OBJS) 

ac: $(AC_OBJS)
	$(CC) $(LDFLAGS) -o $@ $(AC_OBJS) 

mtr: $(MTR_OBJS)
	$(CC) $(LDFLAGS) -o $@ $(MTR_OBJS) 

clean:
	-rm -f $(EXEC) *.elf *.gdb *.o

